# Unet-Baseline-Pytorch
<br/>
Implementation of the baseline Unet architecture in Pytorch [Original Unet Paper](https://arxiv.org/abs/1505.04597)
<br/>
see `Unet_Baseline_pytorch.ipynb` for implemention of dataloader and model.
<br/>
## Overview
<br/>
**Dataset and augmentation**
<br/>
The original dataset contains 30 images. This is not enought for training, hence I have performed data augmentation (explained in `Unet_Baseline_pytorch.ipynb`)
You can find all the data (including augmented set along with segmentation mask) in folder data/membrane.
<br/>
See `Unet_Data_augmentation.ipynb` for more details.
<br/>
**Model**
<br/>
The architecture was implemented in pytroch. 
<br/>
**Training**
<br/>
The model was trained for 25 epochs.
Loss function for the training was  a binary crossentropy + dice loss (improves boundary detection/ segmentation).
<br/>
