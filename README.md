# compostnet
Sarah Frost, Bryan Tor, Rakshit Agrawal, Angus G. Forbes

[Link to our paper](https://github.com/sarahmfrost/compostnet/blob/master/CompostNet.pdf)


# Overview of Project:
![WasteBins](https://github.com/sarahmfrost/compostnet/blob/master/figures/WasteBins.png)

It can be confusing to know what pieces of waste go in which bin. Many businesses, cafes, and outdoor spaces provide trash, recycling, and composting bins, requiring consumers to decipher instructional text, icons, or images in order to sort their waste accurately. Moreover, different locations may have different rules for how to separate waste, and often people inadvertently throw their trash in the wrong bin. Machine learning solutions can help us more quickly and accurately choose the proper receptacle for our waste by classifying a photograph of the waste. Building on recent work in deep learning and waste classification, we introduce CompostNet, a convolutional neural network that classifies images according to how they should be appropriately discarded. We provide details about the design and development of CompostNet, along with an evaluation of its effectiveness in classifying images of waste. Further, we discuss two different approaches to the design of our system, one using a custom network and the other augmenting a pre-trained image classification network (MobileNet) through transfer learning, and finding greater success with the transfer learning approach. To the best of our knowledge, CompostNet is the first waste classification system that uses a deep learning network to identify compostable, recyclable, and landfill materials. CompostNet is an application of machine learning for social good, and supports [United Nations Sustainable Development Goal 12: Responsible Consumption and Production](https://www.un.org/sustainabledevelopment/sustainable-consumption-production/).


## Installation

**Dataset:**
We took the dataset built by Gary Thung and Mindy Yang for [TrashNet](https://github.com/garythung/trashnet) and added a compost class. 

We added 175 photos to the compost class, and added 49 photos to the trash class. We followed the data collecting methods outlined in Trashnet. We resized our images to 400×300 pixels. In the code for our Version A model, we resize the images to 224 × 224 pixels.

Our dataset was too large to upload to github, all data can be found on Google Drive.

[Our Dataset for Version A](https://drive.google.com/drive/folders/1HFouUVZ-bEEi0x_N89cFX0fEBs560STu?usp=sharing)

[Our Dataset for Version B](https://drive.google.com/drive/folders/1lj5JMvcZqV_S7oOou6uWi7ElXWy_pGc5?usp=sharing)


**Code:** 

Version A:

You will need:

Python 3.5

Tensorflow

```
pip install --upgrade "tensorflow==1.7.*"
```

Folders: scripts, tf_file (on google drive) 

Dowload these folders and move them into the same directory

To retrain, change the image_dir path to the path with the training data in commands.txt
to test run the second set of code with an image path from the testing data in commands.txt

Version B we built and ran our code in Google Colab, which can be found in this repo. You can access the notebook with Google Colab or the Jupyter notebook environment.


## Architecture

Version A Architecture

![VersionA Architecture](https://github.com/sarahmfrost/compostnet/blob/master/figures/VersionA_Architecture.png)


Version B Architecture

![VersionB Architecture](https://github.com/sarahmfrost/compostnet/blob/master/figures/VersionB_Architecture.png)


## Results

Version A Accuracy and Results

![VersionA Accuracy](https://github.com/sarahmfrost/compostnet/blob/master/figures/VersionA_Accuracy.png)
![Results](https://github.com/sarahmfrost/compostnet/blob/master/figures/Results1.png)
![More Results](https://github.com/sarahmfrost/compostnet/blob/master/figures/Results1.png)

Version B Accuracy

![VersionBAccuracy](https://github.com/sarahmfrost/compostnet/blob/master/figures/versionB_Accuracy.png)


## Deployment

We are in the process of building a mobile app for deploying this solution.


## Credits

[TrashNet](https://github.com/garythung/trashnet) - Gary Thung and Mindy Yang


