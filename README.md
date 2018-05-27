# Semantic Segmentation
### Results
[//]: # (Image References)

[image1]: ./runs/1527436541.057375/um_000000.png "Road Results"
[image2]: ./runs/1527436541.057375/um_000058.png "Road Results"
[image3]: ./runs/1527436541.057375/um_000040.png "Road Results"
[image4]: ./runs/1527436541.057375/um_000028.png "Road Results"
[image5]: ./runs/1527436541.057375/um_000042.png "Road Results"
[image6]: ./runs/1527436541.057375/uu_000097.png "Road Results"
[image7]: ./runs/1527436541.057375/uu_000098.png "Road Results"
[image8]: ./runs/1527436541.057375/uu_000080.png "Road Results"

#### Results of 6 epochs

![alt text][image1]

![alt text][image2]

![alt text][image3]

![alt text][image4]

![alt text][image5]

![alt text][image6]

![alt text][image7]

![alt text][image8]

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
