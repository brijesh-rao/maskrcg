# mask recognition

This program will first detect a face using a basic cv2 algorithm. An image of this face will then be passed along a pipeline which extracts certain features –more on these under the “Detailed Design of Features” section— and feeds it into a model that can determine (classify) if a mask is present or not. 

## Dataset  

The below dataset is used:  
It has to classes of images one with mask correctly worn other with mask incorrectly worn, all img are 1024* 1024 resolution.
https://github.com/cabani/MaskedFace-Net 

## Detailed Design of Features  

There are a total of five feature extractions currently coded; they are listed below: 

    Canny edge detection 
    Sobel edge detection 
    Harris corner detection 
    Fast detector 
    Laplacian of Gaussian (a blob detector) 

# DONE
Implement a classifier to classify the images from the above feature vectors.

After we have implemented the classifier, we can derive metrics as to which of the feature vectors from the above results in the best fit for the data, in terms of accuracy and performance. 
