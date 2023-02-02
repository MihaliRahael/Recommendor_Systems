# Fashion Recommendor System using ResNet-50

## Problem Statement : To design an Image Search Engine application which recieves a product image and recommends similar products.

### Dataset : https://www.kaggle.com/datasets/vikashrajluhaniwal/fashion-images 

### Approach
We will make use of ResNet-50 architecture. Residual Network (ResNet) is a supervised deep learning model used for computer vision applications. It is a Convolutional Neural Network (CNN) architecture designed to support hundreds or thousands of convolutional layers. Find the architecture below.

![image](https://user-images.githubusercontent.com/106816732/216128908-50dfa641-8304-41a8-aff7-d4c7908230bd.png)

<img width="500" alt="image" src="https://user-images.githubusercontent.com/106816732/216129487-f37131e8-51f8-4aab-b574-ea2981f28b8a.png">

Our dataset contains 6000 images, so we will have 6000 feature vector from ResNet-50 model and 6000 filenames corresponding to each feature vector.

##### How the testing happens?

Once a test image is inputted, the model gives a 2048 output vector. We already have a vector space of training images. So once the test image vector arrives at the space, the  decision will be taken based on the Euclidean distance calculation using KNN.

<img width="508" alt="image" src="https://user-images.githubusercontent.com/106816732/216130264-8679e653-9cce-4bc5-b02b-e0d35caa7fae.png">
