# Mask-R-CNN-MindSpore
A Mindspore version of Mask R-CNN, trained on GPU.

# Mask R-CNN

Mask R-CNN extends Faster R-CNN by adding a branch for predicting segmentation masks on each Region of Interest (RoI), in parallel with the existing branch for classification and bounding box regression. The mask branch is a small FCN applied to each RoI, predicting a segmentation mask in a pixel-topixel manner. Mask R-CNN is simple to implement and train given the Faster R-CNN framework, which facilitates a wide range of flexible architecture designs. Additionally, the mask branch only adds a small computational overhead, enabling a fast system and rapid experimentation. 

![framework](./images/framework.png)

Without bells and whistles, Mask R-CNN surpasses all previous state-of-the-art single-model results on the COCO instance segmentation task, including the heavilyengineered entries from the 2016 competition winner in 2018.

## Model Features
1. Mask R-CNN adds a branch of Mask prediction on the basis of Faster R-CNN\
2. Mask R-CNN proposes ROI ALign.

## Pretrained Model

|  model | training dataset | bbox | segm | ckpt |
|  ----  | ----  | ---- | ---- | ---- |
| maskrcnn_coco2017_bbox37.4_segm32.9 | coco2017 | 0.374 | 0.329 | checkpoint/maskrcnn_coco2017_acc32.9.ckpt |
| maskrcnnmobilenetv1_coco2017_bbox22.2_segm15.8 | coco2017 | 0.222 | 0.158 | checkpoint/maskrcnnmobilenetv1_coco2017_bbox24.00_segm21.5.ckpt |
