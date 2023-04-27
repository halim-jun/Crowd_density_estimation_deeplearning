# Crowd_density_estimation_deeplearning
Model that detects the crowd density from surveilence camera image to prevent crowd crush

## Motivation
- A crowd crush is a disaster where an extremely dense population ends up stumbling into each other, causing severe injuries or deaths on a large scale. On 2022 October 1st, a fatal crush occured in East Java, Indonesia, during a football match, causing more than 135 deaths. 

- Under the purpose of developing a crowd density estimation system to further prevent crowd crush, this project suggests using deep learning models to develop crowd density estimation of image data.

## Model

### Auto encoder
- Convolutional AutoEncoder was deployed in order to make a deep learning model that returns a reconstructed version of the original image into a heatmap, where the densely populated parts are highlighted. 
- This model aims to solve a regression problem where the pixel value of the heatmap of crowd density is the target.

### Sementic Segmentation
- This model solves a classification problem since it assigns each pixel with a certain class of objects to cluster the pixel into. (Whether it is a human or not)


### Density estimation
- From the model output of Sementic Segmentation, regression modeled of crowd density was conducted.
