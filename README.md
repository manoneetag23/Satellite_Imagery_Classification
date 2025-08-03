# Satellite_Imagery_Classification 
Using Deep Learning Satellite RGB images were trained and Classification task was performed. 

## Dataset: 
### Dataset Link : https://zenodo.org/records/7711810/files/EuroSAT_RGB.zip
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

## Model Architecture: 
The model architecture involves
Convolutional Neural Network layers
ReLU activation Fucntion
MaxPooling 
Softmax classifier for multiclass classification
