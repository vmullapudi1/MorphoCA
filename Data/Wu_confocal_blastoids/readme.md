# Input blastoid image files

This folder contains the raw input .nd2 files of the blastoids.
They are used in the pipeline to produce cell centroids via image segmentation.

## Image channel info

| Biomolecule  | Label    | Display Color | Description
| :----------- | :------  | :----         | :-----------
| Oct4         |   GFP    | Green         | Pluripotent Stem Cell Marker
| iYAP         |   TRITC  | Yellow        | Hippo pathway (YAP/TAZ) - mechanosensor (size/profileration regulation)
| Phalloidin   |   Cy5    | Red           | Actin Label
| DAPI         |   DAPI   | Blue          | Nuclear Label
