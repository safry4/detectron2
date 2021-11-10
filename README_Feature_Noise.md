**This repository is a copy of Facebook's detectron2 with following modifications:**

1. Noise-Feature added to FPN (detectron2/modeling/backbone/fpn.py)

2. Plots representing training loss with and without Feature-Noise is added.

# Instructions:

1. Download Coco dataset and transform it according instructions here (https://github.com/facebookresearch/detectron2/blob/main/datasets/README.md)
The data format should be in .json format: train_2017.json under coco/annotations folder.

2. Run plain_train_net.py with configuration:
train_net.py --num-gpus 8 \ --config-file ../configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_1x.yaml