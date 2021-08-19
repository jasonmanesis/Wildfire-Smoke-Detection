[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/JasonManesis/Convolutional-Neural-Network-Classifier-MNIST/blob/main/CNN_MNIST_PyTorch_VISUALS.ipynb)

# Wildfire Smoke Detection.
**Convolutional neural network model based on the architecture of the Faster-RCNN for wildfire smoke detection.**

## Dataset Properties.
<div align="center">
 
This dataset is released by **AI for Mankind** in collaboration with **HPWREN**.

This dataset is licensed under the **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License**.


To learn more about this dataset and its possible applications in fighting wildfires, see this case study of Abhishek Ghosh's wildfire detection model.
The goal is to curate wildfire smoke datasets to enable open sharing and ease of access of datasets for developing vision based wildfire detection models. Easy access and open sharing of datasets will facilitate and accelerate the research efforts in solving wildfire crisis.

HPWREN Cameras
AI For Mankind downloaded the public domain HPWREN Cameras images and annotated these images with bounding boxes for object detection.

Bounding Box Annotated Wildfire Smoke Dataset (Pascal VOC annotation format) Version 1.0 for smoke detection. Thank you our founder Wei Shung Chung in creating this first set of bounding boxes. In total, 744 bounding box annotated images are created.

Bounding Box Annotated Wildfire Smoke Dataset (Pascal VOC annotation format) Version 2.0 This is the latest annotated images we created with the help of our volunteers. It has 2192 annotated images.

Please give credits to AI For Mankind and HPWREN when using these bounding box annotated smoke datasets. The bounding box annotated smoke datasets are licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License.

https://public.roboflow.com/object-detection/wildfire-smoke
 
</div align="center">

## Model Architecture

![](/model_architecture.png)

## Model Performance
 
 Performance Metrics:

|          Metric        |         IoU     |      Area   |      maxDets |   Score  |
|:----------------------:|:---------------:|:-----------:|:------------:|:--------:|
|Average Precision  (AP) |0.50:0.95        |    all      | 100          | **0.547**|
|Average Precision  (AP) |0.50             |    all      |100           | **0.909**|
|Average Precision  (AP) |0.75             |    all      | 100          | **0.561**|
|Average Precision  (AP) |0.50:0.95        |  small      | 100          | **0.318**|
|Average Precision  (AP) |0.50:0.95        | medium      | 100          | **0.497**|
|Average Precision  (AP) |0.50:0.95        | large       |         100  | **0.646**|
|Average Recall     (AR) |0.50:0.95        | all         | 1            | **0.615**|
|Average Recall     (AR) |0.50:0.95        | all         |10            | **0.620**|
|Average Recall     (AR) |0.50:0.95        | all         | 100          | **0.620**|
|Average Recall     (AR) |0.50:0.95        | small       | 100          | **0.443**|
|Average Recall     (AR) |0.50:0.95        | medium      | 100          | **0.584**|
|Average Recall     (AR) |0.50:0.95        | large       | 100          | **0.707**|


## Results
### Images:


Solarized dark                                                    |     Solarized Ocean
:----------------------------------------------------------------:|:-------------------------:
<img width="500" height="400" src="/Images/Results_image_1.png">  |  <img width="500" height="400" src="/Images/Results_image_2.png">



### Videos:


https://user-images.githubusercontent.com/74200033/130096189-c42585e5-79ea-4cef-aa5f-cace7345a81b.mp4



## Requirements

:green_square:  **Pandas == 1.3.2**

:green_square:  **PyTorch**

:green_square:  **Seaborn**

:green_square:  **NumPy**
 
:green_square:  **Seaborn**

:green_square:  **Matplotlib**

    Pandas == 1.3.2                 Pandas == 1.3.2                 Pandas == 1.3.2
    Pandas == 1.3.2                 Pandas == 1.3.2                 Pandas == 1.3.2
    Pandas == 1.3.2                 Pandas == 1.3.2                 Pandas == 1.3.2
    Pandas == 1.3.2                 Pandas == 1.3.2                 Pandas == 1.3.2
    Pandas == 1.3.2                 Pandas == 1.3.2                 Pandas == 1.3.2
    Pandas == 1.3.2                 Pandas == 1.3.2                 Pandas == 1.3.2
    
 
 
