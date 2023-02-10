---
title: Off-Road Open Desert Trail Detection (O2DTD) Dataset
layout: page
permalink: /datasets/offroad/
show_menu: false
---
<img src="/assets/O2DTD_Dataset_Demo_cropped.gif"/>
<h1 style="text-align:center"> <a href="https://1drv.ms/u/s!As-rscCX5HkvkHXf5vx7BMQ7dMqc?e=NjeVGb/"> Download here </a></h1>


Autonomous vehicle technologies rely heavily on freespace detection for visual perception and route planning. In the preceding decade, it was demonstrated that freespace detection methods based on deep learning are viable. However, these attempts primarily dealt with urban on-road environments, and few deep learning-based algorithms were developed for free space detection in off-road scenarios. Nevertheless, to our knowledge, no work has been reported for detecting desert freespace due to the absence of relevant datasets and benchmarks. For research purposes, we curated a new dataset named Off-Road Open Desert Trail Detection (O2DTD), which is the first dataset on desert freespace detection. The dataset was collected with six different light conditions (dawn, morning, afternoon, sunset, twilight, and night), containing a total of 5,045 RGB images, as summarized in Table I. Moreover, as can be seen in the attached demo, each image is labeled with three classes consisting of the sky (blue), ground (brown), and trail (gray) regions.

Table I: Summary of the proposed off-road open desert trail detection (O2DTD) dataset

|Type|Original Images|Labels|Split Ratio|
| :-: | :-: | :-: | :-: |
|||RGB|Single     Channel|Train (70%)|Val (10%)|Test (20%)|
|Dawn|813|813|813|569|81|163|
|Morning|865|865|865|606|87|172|
|Afternoon|922|922|922|645|92|185|
|Sunset|907|907|907|635|91|181|
|Twilight|694|694|694|486|69|139|
|Night|844|844|844|591|84|169|
|Total|5,045|5,045|5,045|3,532|504|1,009|

All the images and ground truth labels in the dataset are stored in PNG format with 360×480 resolution, making it easy to use. Besides, we have randomly split the dataset for each illumination condition in the ratio of 70:10:20 for training, validation, and testing purposes of the model. These images and labels are stored separately in sub-folders inside the main directory, “O2DTD Dataset”. Further, we have provided the ground truth labels in two formats (single channel and RGB). Table II provides the annotation details.

Table II:  Ground truth annotation details for the O2DTD dataset

|Class|Single Channel|RGB|
| :-: | :- | :-: |
||Pixel Value|Color Palette|
|Sky|1|(77, 190, 238)|
|Ground|2|(160, 130, 95)|
|Trail|3|(160, 160, 160)|


*Steps to Use the O2DTD Dataset:*

- Download the O2DTD dataset into the main directory.
- Use the images and ground truth labels provided in the “Training” and “Validation” folders for network training and validation.
- For ground truth annotation details of the O2DTD dataset, please see Table II. 
- Once the model is trained, evaluate it using the images and ground truth labels provided in the “Test” folder.

_Credit: Dr. Bilal Hassan and Hamad Al Remeithi_