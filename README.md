# G-17-Image-Caption-Generator

## Introduction:

Image Captioning is the system of producing a textual description for given images.It has been an extremely important and basic endeavor in the 
Deep Learning space. Picture subtitling has a major amount of use. NVIDIA is the usage of picture captioning applied sciences to create an software to assist human beings who have low or no eyesight.
Picture inscribing can be considered as a start to finish Sequence to Sequence issue, as it changes over pictures, which is considered as a grouping of pixels to a succession of words. For this reason, we need to methodology each the 
language or explanations and the pictures. For the Language part, we utilize intermittent Neural Networks and for the Image part, we use Convolutional Neural Networks to individually accomplish the capacity vectors.
Before moving to further chapters let’s understand the about digital imagers and their advantages.An image is visual representation of object. It can be anything from paintings, sculptures, photos etc. The images are in existence from a very 
long time now. As computers cannot understand images, it became necessary to develop special methods to represent images in computers.


To build this system we followed following architecture where we maintain 2 repositories one of image and other of images's corresponding captions.
We pass images and captions through image and language pipeline respectively. Image pipeline is basically a 2 step process of resizing image to 224x224 
image and passing it through Resnet50 model to generate feature vectors.
In language pipeline, we pass captions and first preprocess them to produce all lower case text, add suffix and prefixes as well. Then captions are passed through
RNN models to generate word embeddings and thus feature vectors.
Both image and caption feature vectors are then passed through LSTM architecture to build a model.

Once model developed, the site is build on Flask framework which is a light-weight python framework.



## Getting Started:
Clone the repo

Download and install python from https://www.python.org/downloads/
Install and update pip to latest version

Install requirements.txt file  
using pip3 install -r requirements.text

To start the application run app.py file
>python3 app.py
This will start the server on localhost
Open http://127.0.0.1:5000 and you will be presented with a running application



## To run training module
Clone the repo

Download and install python from https://www.python.org/downloads/
Install and update pip to latest version

Install requirements.txt file using 
pip3 install -r requirements.text

Download dataset from https://www.kaggle.com/datasets/srbhshinde/flickr8k-sau
run train.py using 
python3 train.py


## The Team:
1. Gaurav Pratap Singh (Roll No :2000520139002, Mobile No :9761321308, email :2000520139002@ietlucknow.ac.in)
2. Apoorv Jha (Roll No :2000520139001, Mobile No :8917096780, email :2000520139001@ietlucknow.ac.in)
3. Mradul dixit(Roll No :1900520130031, Mobile No :8979907283, email :1900520130031@ietlucknow.ac.in)

