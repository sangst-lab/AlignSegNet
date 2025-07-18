# AlignSegNet
This is the source code for paper "AlignSegNet: Registration-Enhanced Segmentation of Prostate Cancer in B-mode Ultrasound Images"

<div align=center><img width="800" height="300" src="https://github.com/sangst-lab/AlignSegNet/blob/main/figures/Figure_1.jpg"/></div>
  <figcaption style="text-align:left; font-size:0.85em; line-height:1.4;">
    <small>
      <strong>Figure 1. Illustration of the MRI–TRUS fusion‑guided biopsy and data fusion.</strong>  
      (a) Illustration of the MRI–TRUS fusion‑guided biopsy workflow. (b) Illustration of MRI–TRUS image fusion using different strategies.
    </small>
  </figcaption>

<div align=center><img width="1200" height="380" src="https://github.com/sangst-lab/AlignSegNet/blob/main/figures/Figure_2.jpg"/></div>
<p align="left"> 
The overview of our method. 
</p>

## Requirements
* albumentations==1.0.0
* inplace_abn==1.1.0
* matplotlib==3.4.2
* numpy==1.22.2
* opencv_python_headless==4.5.2.54
* pretrainedmodels==0.7.4
* segmentation_models_pytorch==0.2.0
* torch==1.8.0
* torchvision==0.9.0

## Data
In order to make it easier for the readers to reproduce and understand the code, I have provided a small amount of example data used in our experiment under the **dataset** folder, where provides six training, validation and test images.

## File declaration


**main.py**: The codes for training, validating and testing.

## Run the codes
Install the environment.
```bash
pip install -r requirements.txt
```

Train and test the model.
```bash
python main.py
```
