# Wildfire Smoke Detection.
Convolutional neural network model based on the architecture of the **Faster-RCNN** for wildfire smoke detection. For this project we used a pretrained model on ImageNet dataset, from detectron2's [Model Zoo](https://detectron2.readthedocs.io/en/latest/modules/model_zoo.html), and fine-tuned it for the task of wildfire smoke detection from optical image data.

## Dataset Properties.
<div align="left">
 
This dataset is released by **AI for Mankind** in collaboration with **HPWREN** (High Performance Wireless Research and Education Network), and is licensed under the [**Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License**](https://creativecommons.org/licenses/by-nc-sa/4.0/). 
 
 **AI For Mankind** is a 501(c)(3) nonprofit organization with the mission of mobilizing the tech community to work on world challenging problems using AI and Data. We organize tech talks, workshops, and hackathons. We want to build a grassroot community of volunteers creating solutions using AI and Data to bring positive impacts to society at large.      (https://aiformankind.org/) 
 
The **High Performance Wireless Research and Education Network (HPWREN)**, a University of California San Diego partnership project led by the San Diego Supercomputer Center and the Scripps Institution of Oceanography's Institute of Geophysics and Planetary Physics, supports Internet-data applications in the research, education, and public safety realms. (http://hpwren.ucsd.edu/)
 
 
The above dataset is available in **2** different versions in **Pascal VOC** annotation format:
 
Bounding Box Annotated Wildfire Smoke Dataset Version 1.0 with **744** annotated images. 
 
 :arrow_right_hook: [ **BBAWS Dataset v1.0 - Pascal VOC**](https://drive.google.com/file/d/1sEB77bfp2yMkgsSW9703vwDHol_cK6D5/view?usp=sharing)
 
 Bounding Box Annotated Wildfire Smoke Dataset Version 2.0 with **2192** annotated images. 
 
:arrow_right_hook: [ **BBAWS Dataset v2.0 - Pascal VOC**](https://drive.google.com/drive/folders/1IKXN2-hxTrEQsIIKOxiUAuLgoxubA9Wq?usp=sharing)

The **first version** of the dataset is also available in **COCO** annotation format by [**Roboflow**](https://roboflow.com/):
 
:arrow_right_hook: [ **BBAWS Dataset v1.0 - COCO**]( https://public.roboflow.com/object-detection/wildfire-smoke)
 


_For this project we used the dataset in **COCO** annotation format provided by Roboflow._

</div align="left">

## Model Architecture
The model architecture is based on the general architecture of the **Faster-RCNN**, which includes the main modules of **Feature Pyramid Network**, **Region Proposal Network** as well as the model of **Fast-RCNN**. For the bottom-up pathway of the FPN network the architecture of the **ResNet50** was used.

<img src="https://miro.medium.com/max/2000/1*Wvn0WG4XZ0w9Ed2fFYPrXw.jpeg">

_Image source: https://miro.medium.com/max/2000/1*Wvn0WG4XZ0w9Ed2fFYPrXw.jpeg_


## Model Performance

|          **Metric**        |         **IoU**     |      **Area**   |      **maxDets*** |   **Score**  |
|:--------------------------:|:-------------------:|:---------------:|:-----------------:|:------------:|
|Average Precision  (AP)     |0.50:0.95            |    all          |100                |     **0.551**|
|Average Precision  (AP)     |0.50                 |    all          |100                |     **0.921**|
|Average Precision  (AP)     |0.75                 |    all          |100                |     **0.582**|
|Average Precision  (AP)     |0.50:0.95            |  small          |100                |     **0.333**|
|Average Precision  (AP)     |0.50:0.95            | medium          |100                |     **0.495**|
|Average Precision  (AP)     |0.50:0.95            | large           |100                |     **0.660**|
|Average Recall     (AR)     |0.50:0.95            | all             | 1                 |     **0.604**|
|Average Recall     (AR)     |0.50:0.95            | all             |10                 |     **0.608**|
|Average Recall     (AR)     |0.50:0.95            | all             | 100               |     **0.608**|
|Average Recall     (AR)     |0.50:0.95            | small           | 100               |     **0.429**|
|Average Recall     (AR)     |0.50:0.95            | medium          | 100               |     **0.568**|
|Average Recall     (AR)     |0.50:0.95            | large           | 100               |     **0.700**|

*_Maximum number of detections per image._

**Download final model [`HERE`](https://drive.google.com/file/d/12TmbotrgL8q5R7u7pMuN34cnA_-4cGia/view?usp=sharing) (≈158.6 MB)** 

## Results

https://user-images.githubusercontent.com/74200033/130357982-c47f46ed-af8a-48c1-abeb-d4761eb707c6.mp4

**Original video at:** https://www.youtube.com/watch?v=q07TBd5o1HQ&t=35s

https://user-images.githubusercontent.com/74200033/130357983-04dbce41-5e87-456c-ad55-a9769d1ec1d5.mp4

**Original video at:** https://www.youtube.com/watch?v=5cEr5ZXGUYA    

**Download full results [`HERE`](https://drive.google.com/drive/folders/1wakQ7tUbXv-_HZX56l5C_tGunGw2CmaS?usp=sharing) (≈589 MB)**  

## Requirements

    torch == 1.9.0+cu102                           numpy == 1.19.5                           json == 2.0.9
    torchvision == 0.10.0+cu102                    yaml == 5.1                               fiftyone == 0.12.0
    pyyaml == 5.1                                  pandas == 1.3.2                           IPython == 5.5.0
    detectron2 == 0.5                              cv2 == 4.1.2
                  
  
