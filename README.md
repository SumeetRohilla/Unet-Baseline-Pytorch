# Unet-Baseline-Pytorch

Implementation of the baseline Unet architecture in Pytorch [Original Unet Paper](https://arxiv.org/abs/1505.04597)

see [Unet_Baseline_pytorch.ipynb](https://nbviewer.jupyter.org/github/SumeetRohilla/Unet-Baseline-Pytorch/blob/master/Unet_Baseline_pytorch.ipynb) for implemention of dataloader and model.
Dataloader was built using the techniques taught in FastAI course 2.

**Overview**

**Dataset and augmentation**

The original dataset contains 30 images. This is not enought for training, hence I have performed data augmentation to increase the dataset size.
You can find all the data (including augmented set along with segmentation mask) in folder data/membrane.

See [Unet_Data_augmentation.ipynb](https://nbviewer.jupyter.org/github/SumeetRohilla/Unet-Baseline-Pytorch/blob/master/Unet_Data_augmentation.ipynb) for more details.

**Model**

The architecture was implemented in pytroch. 

**Training**

The model was trained for 25 epochs (batch size =1).
Loss function for the training was  a binary crossentropy + dice loss (improves boundary detection/ segmentation).
