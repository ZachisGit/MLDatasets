# MLDatasets
Python library that hosts/formats datasets.

This is going to be a easy to use ML dataset hosting/formating library intended to make it easy to download/preprocess/format/etc. your datasets.

# First Steps
The first area that will be targeted are image based datasets for classification, image segmentation, image translation and object detection (bounding boxes).
Now the first thing that has to happen is the creation of a image based dataset index. If you know of or use any image based datasets not in the index yet, please consider adding them. The format of the index is very simple (see Image Based Dataset Index).

# Image Based Dataset Index
The image based dataset index file can be found in /datasets/image_based.idx<br/>
<br/>
<b>Format:</b><br/>
[Dataset Name];[Dataset Type];[Additional information];[Dataset Download Url]\n
<br/>
<br/>
Dataset Name = that is just the name of the dataset<br/>
Dataset Type = there are different types of datasets, not sure on these yet so make up your own (e.g bounding_boxes, classification,etc.)<br/>
Additional Information = any infos you have (like a description)<br/>
Dataset Download Url = the direct url/urls to download the dataset (if there are multiple files to be downloaded provide all urls seperated with ';')<br/>
<br/>
<b>Format-Example:</b><br/>
[...]<br/>
horse2zebra;unsupervised_image_translation;dataset used in the cyclegan paper for unsupervised horse to zebra image translation;https://people.eecs.berkeley.edu/~taesung_park/CycleGAN/datasets/horse2zebra.zip<br/>
[...]<br/>
<br/>
<b>MNIST-Example (multiple urls seperated with ';'):</b><br/>
[...]<br/>
mnist;classification;digit classification 0-9 (info link: http://yann.lecun.com/exdb/mnist/) ;http://yann.lecun.com/exdb/mnist/train-images-idx3-ubyte.gz;http://yann.lecun.com/exdb/mnist/train-labels-idx1-ubyte.gz;http://yann.lecun.com/exdb/mnist/t10k-images-idx3-ubyte.gz;http://yann.lecun.com/exdb/mnist/t10k-labels-idx1-ubyte.gz
<br/>
[...]<br/>
