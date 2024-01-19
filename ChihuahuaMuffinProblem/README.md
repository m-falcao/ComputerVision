# *Chihuahua Blueberry Muffin Problem*

### This code is a solution for a machine learning problem that aims to differentiate between images of chihuahua dogs and blueberry muffins. It is written in Python and runs on a Jupyter Notebook in Google Colab.

## Setup
The code requires several Python packages to be installed. The following packages can be installed by running the commands:
- pip install requests
- pip install bs4
- pip install fastcore
- pip install fastdownload
- pip install fastai

## Usage
The code starts by creating a temporary directory to download and store the images.

It then downloads images of chihuahua dogs and blueberry muffins from the internet using the search_images function and saves them in the temporary directory using the download_images_word function.

The downloaded images are then resized to a maximum size of 400 pixels using the resize_images function.

The script then creates data loaders using the DataBlock class from the fastai.vision.all module.

A model is trained using the fine_tune method of a learner object from the fastai.vision.all module.

Finally, the model is tested on a randomly selected image from each category, and the predicted category and the probabilities of the predictions are printed.

## Limitations
Due to the limit imposed by the Google API, only a maximum of 20 images can be downloaded for each search term. This may limit the accuracy of the model.
