# Osdag_FOSSEE_2026
*This repository contains a Python-based structural post-processing workflow to generate 2D and 3D Shear Force Diagrams (SFD) and Bending Moment Diagrams (BMD) for a bridge finite element model. The visualizations are designed to closely replicate MIDAS-style post-processing output.**

The project:

Reads FEM results from a NetCDF (.nc) file using Xarray

Extracts internal forces (Mz, Vy) at element end nodes

Ensures element continuity and sign consistency

Generates:

2D SFD and BMD for individual girders

3D MIDAS-style SFD and BMD for all girders

How to Run:
  1. Place the FEM result file in the project directory:
  2. Run the notebook or script to:
          Generate 2D SFD & BMD
          Generate 3D SFD & BMD for all girders
  3. Switch between diagrams by changing:
       component="Mz"  # BMD
       component="Vy"  # SFD
