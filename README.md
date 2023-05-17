# RIS on Fashion Data
## Description
Final project of BIG Data course: Reverse Image Search on Fashion Data

There are two notebooks:

* [Model_Fine-Tune.ipynb](Model_Fine-Tune.ipynb)
* [Reverse_Image_Search_on_Fashion_Data.ipynb](Reverse_Image_Search_on_Fashion_Data.ipynb)

The main one is [Reverse_Image_Search_on_Fashion_Data.ipynb](Reverse_Image_Search_on_Fashion_Data.ipynb), additional notebook for model training is: [Model_Fine-Tune.ipynb](Model_Fine-Tune.ipynb).

## Data

The dataset is taken from here: [https://github.com/alexeygrigorev/clothing-dataset](https://github.com/alexeygrigorev/clothing-dataset). Smaller dataset with 10 different classes of clothes is used for this project. 

## Purpose 

The purpose of the project is to create a ML algorithm, which, given one image, searches for the most similar images having no additional information about them.

## Searching for similar images

We convert every image  to feature vector using different neural network models, and then compute distances (cosine and euclidean) between target image feature vector and  all the saved feature vectors to find best matching images. We use ResNet50V2 pre-trained model, fine-tune it, add some augmentations. 

## Results

We achieved the best results by fine-tunning model and adding augmentations to the data. Our data is labeled. We assume, that our predicted value is most common class of 5 similar images. As a main metric we use accuracy. Accuracy of 87%  was achieved on the test dataset.
