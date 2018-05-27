# Semantic Segmentation
### Results
[//]: # (Image References)

[image1]: ./runs/1527426696.3337421/umm_000066.png "Road Results"
[image2]: ./runs/1527426696.3337421/umm_000066.png "Road Results"
[image3]: ./runs/1527426696.3337421/umm_000066.png "Road Results"

![alt text][image1]

![alt text][image1]

![alt text][image1]
### Introduction
In this project, you'll label the pixels of a road in images using a Fully Convolutional Network (FCN).

### Setup
##### GPU
`main.py` will check to make sure you are using GPU - if you don't have a GPU on your system, you can use AWS or another cloud computing platform.
##### Frameworks and Packages
Make sure you have the following is installed:
 - [Python 3](https://www.python.org/)
 - [TensorFlow](https://www.tensorflow.org/)
 - [NumPy](http://www.numpy.org/)
 - [SciPy](https://www.scipy.org/)
##### Dataset
Download the [Kitti Road dataset](http://www.cvlibs.net/datasets/kitti/eval_road.php) from [here](http://www.cvlibs.net/download.php?file=data_road.zip).  Extract the dataset in the `data` folder.  This will create the folder `data_road` with all the training a test images.

### Start
##### Run
Run the following command to run the project:
```
python main.py
```
##### Implementation details
In this work, FCN-8 that is mentioned in this paper is implemented. [link placeholder]
It consist of a modified VGG network and 1x1 convolutions and deconvolutions to maintain the spatial information of the result of the VGG network.
