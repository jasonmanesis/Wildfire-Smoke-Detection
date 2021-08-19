[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/JasonManesis/Convolutional-Neural-Network-Classifier-MNIST/blob/main/CNN_MNIST_PyTorch_VISUALS.ipynb)

# Wildfire Smoke Detection.
**Convolutional neural network model based on the architecture of the Faster-RCNN for wildfire smoke detection.**

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





    Indent paragraphs to include them in the footnote.

    `{ my code }`

    Add as many paragraphs as you like.
 

## Results
### Images:


Solarized dark                                                    |     Solarized Ocean
:----------------------------------------------------------------:|:-------------------------:
<img width="500" height="400" src="/Images/Results_image_1.png">  |  <img width="500" height="400" src="/Images/Results_image_2.png">



### Videos:


https://user-images.githubusercontent.com/74200033/130096189-c42585e5-79ea-4cef-aa5f-cace7345a81b.mp4



## Requirements

<pre>
 Pandas                                Seaborn                                NumPy                          
 PyTorch                               Matplotlib                             scikit-learn        
                                                                 
</pre> 
