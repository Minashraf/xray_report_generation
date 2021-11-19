# Introduction: X-Ray Report Generation
This repository is for our EMNLP 2021 paper "Automated Generation of Accurate &amp; Fluent Medical X-ray Reports". Our work adopts x-ray (also including some history data for patients if there are any) as input, a CNN is used to learn the embedding features for x-ray, as a result, <B>disease-state-style information</B> (Previously, almost all work used detected disease embedding for input of text generation network which could possibly exclude the false negative diseases) is extracted and fed into the text generation network (transformer). To make sure the <B>consistency</B> of detected diseases and generated x-ray reports, we also create a <B>interpreter</B> to enforce the accuracy of the x-ray reports. For details, please refer to [here](https://arxiv.org/pdf/2108.12126.pdf).

<p align="center">
  <img src="https://github.com/ginobilinie/xray_report_generation/blob/main/img/motivation.png" width="400" height="400">
</p>


# Data we used for experiments
We use two datasets for experiments to validate our method: 

  - [OpenI](https://openi.nlm.nih.gov/)
  - [MIMIC](https://physionet.org/content/mimiciii-demo/1.4/)
  

# Performance on two datasets


# Environments for running codes
   
   - Operating System: Ubuntu 18.04
   
   - Hardware: tested with RTX 2080 TI (11G)

   - Software: tested with PyTorch 1.5.1, Python3.7, CUDA 10.0, tensorboardX, Ninja, tqdm, Easydict
   
   - Anaconda is strongly recommended


# How to use our code for train/test

## How to train

## Our pretrained models

Our model is uploaded in google drive, please download the model from


## How to test

# Citation
If it is helpful to you, please cite our work:
```
@article{nguyen2021automated,
  title={Automated Generation of Accurate$\backslash$\& Fluent Medical X-ray Reports},
  author={Nguyen, Hoang TN and Nie, Dong and Badamdorj, Taivanbat and Liu, Yujie and Zhu, Yingying and Truong, Jason and Cheng, Li},
  journal={arXiv preprint arXiv:2108.12126},
  year={2021}
}
```
