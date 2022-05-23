# VIA_json-file_modification
The output file of Mask R-CNN should be modified to the specific format before compute the AP (PASACAL VOC)
## Converts the format of output file to the specific format
Original output from Mas R-CNN:
* Groundtruth
`{"gt_bbox", "gt_class_id", "image_id"}`

* Prediction Results
`{"rois", "class_ids", "scores", "image_id"}`

`VIA_json_modify.ipynb` output:

`[<left> <top> <right> <bottom>, <confidence>, <image id>]`

## Compute AP 
origin from https://zhuanlan.zhihu.com/p/70667071
