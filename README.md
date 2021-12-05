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

![download (42)](https://user-images.githubusercontent.com/44440114/144754186-23d517f3-64f6-4634-bd58-7d8ec965ef72.png)

Now we can clearly notice from the image that we have 3 clusters i. Nucleus, ii. Cytoplasm and iii. Background
So we use K-Means Clustering algorithm to show the clusters with K=3

## Step 3: Using K-Means Clustering 

![download (43)](https://user-images.githubusercontent.com/44440114/144754236-8e138a94-147f-4a40-8e9c-f453514dd411.png)

The top left represents the original image while the others represent the different clusters formed
Now we take the 2nd image on the first row, since it represents the nucleus and observe it after having used Median Blur

## Step 4: Taking the Nucleus cluster, then Use Median Blur and Thresholding

![download (45)](https://user-images.githubusercontent.com/44440114/144754354-8242c68e-7f63-491f-8d48-6d4ec6ab9f0e.png)

After that we remove the noise using an morphological opening and a closing operation simultaneously

## Step 5: Morphological Operations
![download (46)](https://user-images.githubusercontent.com/44440114/144754399-fef5a357-932d-4827-aaaf-bd7371e3cdd9.png)

Now replace the white pixels with the original pixel from the image 

## Step 6: Output for Segmentation 
![download (47)](https://user-images.githubusercontent.com/44440114/144754433-d48ff7ed-7baf-4328-8fb2-0b158f4e46c8.png)

