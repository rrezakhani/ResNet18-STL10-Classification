# Classification of dataset STL-10 using pretrained Resnet18 in PyTorch

## How to get the dataset STL-10
Image classification of STL-10 dataset, which includes 10 classes of images: airplane, bird, car, cat, deer, dog, horse, monkey, ship, truck. Dataset can be downloaded at: https://cs.stanford.edu/~acoates/stl10/

To download the dataset, use the "stl10_input.py" script on https://github.com/mttk/STL10. Running this script will create the following directories:

**File descriptions** 

 *  /train folder - the training set folder contining 10 subfolders corresponding to each class. Each folder includes 500 images for that class resulting in total 5000 trainig example imgaes. 
 *  /test folder - the test set folder contining 10 subfolders corresponding to each class. Each folder includes 800 images for that class resulting in total 8000 trainig example imgaes. 

## Model
Pretrained Resnet18 is used here, and only its last dense layer is adjusted to the possible 10 classes of STL-10 dataset.

## Effect of data augmentation
Two note books are available to compare the effect of data augmentation. In "ResNet18-STL10.ipynb", several transforms are combined to apply on the training set in order to create additional images to train deep neural network. This will lead to greater number images for model training, which is expected to reduce overfitting.

Comparing the curved of accuracy and loss versus number of epochs, it is confirmed that the data augmentation has resolved overfitting, which is clear in the model with no image transforms. 


https://github.com/rrezakhani/ResNet18-STL10-Classification/tree/main/curves
