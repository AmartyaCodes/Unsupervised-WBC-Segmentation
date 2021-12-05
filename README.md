# Unsupervised-WBC-Segmentation
Segmentation of White Blood Cells using Unsupervised Machine Learning Technique
### Use of K-Means Clustering with Morphological Operations 
## What is K-Means Clustering? 
K-Means Clustering is an unsupervised Machine Learning Technique that uses the concept of euclidean/hamiltonian distance to separate and 
form clusters. 




![download (40)](https://user-images.githubusercontent.com/44440114/144753953-22adddaa-4fed-4110-b01d-053284af4044.png)


Now we would see how we are using K-Means Clustering for Nucleus Segmentation
## Step 1: Image extraction and showing 

![download (41)](https://user-images.githubusercontent.com/44440114/144754057-d4943ed0-7b59-4abb-a9d6-6181b2106e0f.png)

So we get an RGB Image containing multiple White Blood Cells(WBCs), from here we wish to extract both the nucleus and the cytoplasm
And it was found out through experiments, the H channel of the image, converted to HSV color channel, gave the best results.
So 
## Step 2: Giving H channel image as an Output


