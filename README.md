# Classification of dataset STL-10 using pretrained Resnet18 in PyTorch

## How to get the dataset STL-10
Image classification using STL-10 dataset, which includes 10 classes of images: airplane, bird, car, cat, deer, dog, horse, monkey, ship, truck. Data set can be downloaded at: https://cs.stanford.edu/~acoates/stl10/

To download the dataset, use the "stl10_input.py" script on https://github.com/mttk/STL10. Running this script will create the following directories:

**File descriptions** 

 *  /train folder - the training set folder contining 10 subfolders corresponding to each class. Each folder includes 500 images for that class resulting in total 5000 trainig example imgaes. 
 *  /test folder - the test set folder contining 10 subfolders corresponding to each class. Each folder includes 800 images for that class resulting in total 8000 trainig example imgaes. 
