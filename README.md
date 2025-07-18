# AlignSegNet
This is the source code for paper **AlignSegNet: Registration-Enhanced Segmentation of Prostate Cancer in B-mode Ultrasound Images**.

AlignSegNet is an end-to-end deep learning framework that jointly learns image registration and segmentation to accurately localize prostate anatomy and cancerous lesions in real‑time ultrasound (TRUS) by leveraging pre‑acquired MRI information.

<div align=center><img width="800" height="300" src="figures/Figure_1.jpg"/></div>
  <figcaption style="text-align:left; font-size:0.85em; line-height:1.4;">
    <small>
      <strong>Illustration of the MRI–TRUS fusion‑guided biopsy and data fusion.</strong>  
**(a)** Clinical workflow: a radiologist first segments the prostate and lesion on MRI, then maps that annotation onto live TRUS for targeted biopsy.  
**(b)** Naive fusion (top) fails when anatomical structures are misaligned. Applying AlignSegNet (bottom) yields well‑co‑localized prostate boundaries and lesions across both modalities.
    </small>
  </figcaption>


<div align=center><img width="1200" height="380" src="https://github.com/sangst-lab/AlignSegNet/blob/main/figures/Figure_2.jpg"/></div>
<p align="left"> 
<strong>The overview of our method</strong>. Both registration and segmentation components are interchangeable, allowing easy adaptation to other multimodal medical imaging tasks.
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
