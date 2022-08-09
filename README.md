# CellProfiler cellpose detection README

## Data

These pipelines were developed for 2/3D FLIM images of adherent, immune and organoid cancer cells. Images are found in "example_images". The pipeline file are called "runcellposeAdherentCells.cppipe, runcellposeOrganoid.cppipe and runcellposeImmuneCells.cppipe" and is built for use with runCellpose using Cellpose 2.0.
The pipelines will segment the nuclei, whole cell, link the objects and extract the cytoplasm for each cell.

## Instructions

These pipelines require installing cellprofiler from source and downloading and configuring the cellprofiler-plugins repo. Check out the instructions available [on Github](https://github.com/CellProfiler/CellProfiler-plugins).

Note that a GPU is required for the example image to be processed in a timely fashion. If you don't have a GPU, Cellpose will use the CPU.


## Example results

### Cellpose segmentation of nuclei (RunCellpose):
![](/images:README/runCellpose_for_nucleidetection.png)

### Cellpose segmentation of whole cell (RunCellpose):
![](/images:README/runCellpose_for_celldetection.png)

### Find the cytoplasm (IdentifyTertiaryObjects):
![](/images:README/findcytoplasm.png)

### Final segmentation:

![](/images:README/finalresult.png)