# compostnet
Sarah Frost, Bryan Tor, Rakshit Agrawal, Angus G. Forbes

[Link to our paper](https://github.com/sarahmfrost/compostnet/blob/master/CompostNet.pdf)

# Overview of Project:
![WasteBins](https://github.com/sarahmfrost/compostnet/blob/master/figures/WasteBins.png)

It can be confusing to know what pieces of waste go in which bin. Many businesses, cafes, and outdoor spaces provide trash, recycling, and composting bins, requiring consumers to decipher instructional text, icons, or images in order to sort their waste accurately. Moreover, different locations may have different rules for how to separate waste, and often people inadvertently throw their trash in the wrong bin. Machine learning solutions can help us more quickly and accurately choose the proper receptacle for our waste by classifying a photograph of the waste. Building on recent work in deep learning and waste classification, we introduce CompostNet, a convolutional neural network that classifies images according to how they should be appropriately discarded. We provide details about the design and development of CompostNet, along with an evaluation of its effectiveness in classifying images of waste. Further, we discuss two different approaches to the design of our system, one using a custom network and the other augmenting a pre-trained image classification network (MobileNet) through transfer learning, and finding greater success with the transfer learning approach. To the best of our knowledge, CompostNet is the first waste classification system that uses a deep learning network to identify compostable, recyclable, and landfill materials. CompostNet is an application of machine learning for social good, and supports United Nations Sustainable Development Goal 12: Responsible Consumption and Production.


#### Table of Contents
* [Installation](#installation)
* [Running](#running)
* [Results](#results)
* [Deployment Framework](#Deployment Framework)
* [Credits](#credits)

## Installation

To run the project you will need:

 
## Running
Once you have all the depenedencies ready, do the folowing:



## Results


## Deployment Framework
We would like to continue to experiment and test the boundaries of media creation using our Tensorflow implementation. We hope to test the algorithm with a black and white painting for style, while the content style is in color. We also would like continue investigating style subtraction and see if we can achieve more compelling results. This is an implementation of the algorithm in which a section of the style image is removed, and nothing is given to replace it. We would like to investigate how the algorithm harmonizes the empty space with the style of the surrounding image.

In addition, we hope to build a web app that will allow users to upload a piece of art with style and content and harmonize the media with ease. This will allow casual cre- ators to make media. Similar apps exist for style transfer (deepart.io, algorithmia, pikazo, etc.) but an app does not currently exist for style harmonization. This web app would allow users to engage with the Deep Painterly Harmonization algorithm even if they lack the processing power of GPUs or the knowledge of recurrent neural networks.

## Credits

TrashNet - Gary Thung and Mindy Yang
https://github.com/garythung/trashnet


