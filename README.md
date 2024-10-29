# CSC519/791 Course Project: LPRNet_Pytorch Optimization

This repository contains LPRNet model implementation. It is a lightweight License Plate Recognition model. It is adapted from https://github.com/sirius-ai/LPRNet_Pytorch. 

## dependencies

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
The image file base name is the true plate number, that is, the label of the image.
These plates are Chinse plates; the first character of a plate is a Chinese character. 
The training and testing script requires the image size to be 94x24, which is the size of the images in the train and test folders.

## Training and testing

1. Base on your datsets path, modify the parameters --train_img_dirs or --test_img_dirs in the scripts.
2. Adjust other hyperparameters if need.
3. Run 'python train_LPRNet.py' or 'python test_LPRNet.py'.
4. If you want to show the testing result, add '--show true' or '--show 1' flags to the command. 

## References

1. [LPRNet: License Plate Recognition via Deep Neural Networks](https://arxiv.org/abs/1806.10447v1)

