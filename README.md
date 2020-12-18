# Raw Dataset Annotater
These are scripts designed to take sets of images rendered from game engines
(one of which represents the source image, and the other the annotations on
that source image of objects of interest)-- and produce annotated datasets in
various formats for ML training.

There are two versions of these scripts: one in Python, and the other in Rust.
Running details for each of the scripts are in the respective folders. 

## Python
Produces
[Supervisely](https://docs.supervise.ly/data-organization/00_ann_format_navi)
annotations with both bounding box and bitmap annotations.

## Rust
Currently works minimally to produce Supervisely datasets with only bounding
boxes (no bitmap annotations yet).

# Other formats
Supervisely datasets generated with either version can then be further
converted to [Pascal
VOC](https://towardsdatascience.com/coco-data-format-for-object-detection-a4c5eaf518c5)
with [these
scripts](https://github.com/forensic-architecture/scripts/tree/main/to_pascal).

