# Contents
 * Introduction
 * Approach
 * Dataset
 * Output
 * Kaggle Competition (Deep Learning Coursework)

## Introduction
A classification problem solved by training a Convolutional Neural Network, with a goal to predict type of cell for the unlabelled test data, with the trained CNN model. 

## Approach
The results are achieved in the following stages - 
1. Developed a simple CNN that is trained on the labelled train data and evaluated for accuracy with unlabelled test data.
2. With use of autoencoders, the existing CNN model is trained on unlabelled test data.
3. With just using encoder component of the trained autoencoder, the CNN is retrained on a subset of labelled train data and re-evaluated for accuracy.

## Dataset
We have 32x32 image with a cell nuclei needed to be classified into one of the following types:
1. Normal epithelial cells.
2. Cancer epithelial cells.
3. Immune leukocyte cells.
4. Connective fibroblast cells.

In the input directory, we have two sub directories *train* and *test* containing labelled and unlabeled images respectively. 
The *train* folder contains images in relevant class directories - 
```
input/train/train/Cancer
input/train/train/Immune
input/train/train/Connective
input/train/train/Normal
```

## Output
The output was generated in the form of a csv named *test.csv*, with the test data labelled. To check the format of output file, check out the ```input/example.csv```

## Kaggle Competition (Deep Learning Coursework)
As part of our competition styled coursework for the Deep Learning module, this notebook was submitted for evaluation, with guidelines provided by Dr. Kevin Bryson. 
For more details on my submission (Dolphin), visit https://www.kaggle.com/competitions/deep-learning-for-msc-coursework-2022/
