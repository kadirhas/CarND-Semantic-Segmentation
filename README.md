# Semantic Segmentation
### Results
[//]: # (Image References)

[image1]: ./runs/epoch6/um_000000.png "Road Results"
[image2]: ./runs/epoch6/um_000058.png "Road Results"
[image3]: ./runs/epoch6/um_000040.png "Road Results"
[image4]: ./runs/epoch6/um_000028.png "Road Results"
[image5]: ./runs/epoch6/um_000042.png "Road Results"
[image6]: ./runs/epoch6/uu_000097.png "Road Results"
[image7]: ./runs/epoch6/uu_000098.png "Road Results"
[image8]: ./runs/epoch6/uu_000080.png "Road Results"

[image351]: ./runs/epoch35/um_000000.png "Road Results for 35 epochs"
[image352]: ./runs/epoch35/um_000058.png "Road Results for 35 epochs"
[image353]: ./runs/epoch35/um_000040.png "Road Results for 35 epochs"
[image354]: ./runs/epoch35/um_000028.png "Road Results for 35 epochs"
[image355]: ./runs/epoch35/um_000042.png "Road Results for 35 epochs"
[image356]: ./runs/epoch35/uu_000097.png "Road Results for 35 epochs"
[image357]: ./runs/epoch35/uu_000098.png "Road Results for 35 epochs"
[image358]: ./runs/epoch35/uu_000080.png "Road Results for 35 epochs"

#### Results of 6 epochs

![alt text][image1]

![alt text][image2]

![alt text][image3]

![alt text][image4]

![alt text][image5]

![alt text][image6]

![alt text][image7]

![alt text][image8]

#### Results of 35 epochs

![alt text][image351]

![alt text][image352]

![alt text][image353]

![alt text][image354]

![alt text][image355]

![alt text][image356]

![alt text][image357]

![alt text][image358]

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
In this work, FCN-8 that is mentioned in [this paper](https://people.eecs.berkeley.edu/~jonlong/long_shelhamer_fcn.pdf) is implemented. 
It consist of a modified VGG network and 1x1 convolutions and deconvolutions to maintain the spatial information of the result of the VGG network.
