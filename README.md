# Satellite_Imagery_Classification 
Using Deep Learning Satellite RGB images were trained and Classification task was performed. 

### Dataset: 
#### Dataset Link : https://zenodo.org/records/7711810/files/EuroSAT_RGB.zip
The dataset was trained using above RGB Images, Further Data was organised using Train, Test, Validation Folder using "train_test_split"

The dataset was download directly by creating a folder in colab, downloaded in .zip and then extracted using below:

#### Step 1: Create a directory to store the dataset
!mkdir -p /content/satellite_classification

#### Step 2: Download the dataset using wget
!wget -O /content/satellite_classification/EuroSAT_RGB.zip "https://zenodo.org/records/7711810/files/EuroSAT_RGB.zip?download=1"

#### Step 3: Unzip the dataset
!unzip -q /content/satellite_classification/EuroSAT_RGB.zip -d /content/satellite_classification/


## Data Training Setup:
Batch size: 64
Image size: 64x64
Normalization using ImageNet statistics

## Libraries used:
Python
PyTorch
Torchvision
scikit-learn
Matplotlib & PIL
Google Colab or Local GPU (CUDA optional)

## What was Done ?
1. The EuroSAT RGB dataset was downloaded, extracted, and neatly organized into training, validation, and test splits.
2. A custom convolutional neural network (CNN) was built using PyTorch which shows understanding of deep learning workflows.
3. Images were resized to 64×64 and normalized using ImageNet statistics, for better training.
4. Training and validation accuracy/loss were plotted to monitor progress over epochs.
   
## What can be Improved ?
1. Plot histograms of RGB channel intensities. It helps us understand whether image normalization is working effectively or not.
2. A confusion matrix plot would clearly highlight which classes are being confused with each other.
3. Using pretrained models like ResNet can boost performance with fewer data along with faster convergence.
4. Trying classification of Images with higher resolutions like 128x128 and 224x224 as it could help the model capture more details.

## Model Architecture: 
The model architecture involves
Convolutional Neural Network layers
ReLU activation Fucntion
MaxPooling 
Softmax classifier for multiclass classification
