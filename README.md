# CSC519/791 Course Project: LPRNet_Pytorch Optimization

This repository contains LPRNet model implementation. It is a lightweight License Plate Recognition model. It is adapted from https://github.com/sirius-ai/LPRNet_Pytorch. 

## Dependencies

- pytorch >= 1.0.0
- opencv-python 3.x
- python 3.x
- imutils
- Pillow
- numpy

## Pretrained model

* [pretrained_model](https://github.com/sirius-ai/LPRNet_Pytorch/tree/master/weights/)

## Dataset

The data folder contains train and test datasets. The dataset is relatively small, 800 images in train and 200 in test.

The base name of each image file is the plate number, that is, the label of the image.

These plates are Chinse plates; the first character of a plate is a Chinese character. 

The training and testing script requires the image size to be 94x24, which is the size of the images in the train and test folders.

## Training and testing

Run 'python train_LPRNet.py' or 'python test_LPRNet.py' for training and testing respectively.

If you want to show the testing result, add '--show true' or '--show 1' to the above command. 

## References

1. [LPRNet: License Plate Recognition via Deep Neural Networks](https://arxiv.org/abs/1806.10447v1)

