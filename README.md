# Image_Text_Detection_Recognition_Translation

This repository contains:

1. A Jupyter Notebook for detecting and recognizing texts in images. The image detector is built using [EAST: An Efficient and Accurate Scene Text Detector](https://arxiv.org/pdf/1704.03155) and the text recognizer is built using a [CRNN](https://arxiv.org/pdf/1507.05717).
2. Second Jupyter Notebook for Translating text from hindi to english using an [Encoder-Decoder](https://arxiv.org/pdf/1409.0473).

## USAGE
For using the notebooks open both the notebooks in **Google Colab**.

![Sample_Image](https://github.com/nerdishhomosapein/Image_Text_Detection_Recognition_Translation/blob/main/Sample_Image.jpg)

# Project Statement
The goal of this project is to develop a **deep learning** model which translates the text written on a signboard to another language(currently only hindi) as desired by the user. The user will just input an image and then the model should then translate the text written on the signboard. We will first design a system which works for names (such as road names, city names, organisation names shop names etc.) which typically contain 1-2 words and are rarely longer than 4-5 words.


# Dataset
For building such a model, we need a dataset of many images containing some text written in Indian languages(Preferably Hindi). Further, each image should have the following annotations:

1. A bounding box indicating the region containing the text as shown in the images in the LHS figure.

2. The text written inside this bounding box (i.e., a human needs to type out the text)
![Sample-Training-Imge](https://github.com/nerdishhomosapein/Image_Text_Detection_Recognition_Translation/blob/main/Text_Images_Cropped_from_EAST.jpg)

Some existing datasets for Indian language scene text detection are listed below:
1. ICDAR2017
2. https://github.com/lifeisshubh/Awesome-Indic-Scene-Text-Dataset
3. [Word Image dataset for 11 Indian scripts](http://mile.ee.iisc.ernet.in/Downloads/multi.zip)

You can also directly download mine dataset from the google drive links:
1. [Text Detection (Detecting bounding boxes containing text in the images)] (https://drive.google.com/open?id=1Z6Qxr-q-F54iYB2G1AyoDymBh64f5REZ)
2. [Text Recognition (Getting the text from the detected crop) ](https://drive.google.com/open?id=1C0-mc0WAIdssS5KJwOjghaWaqiImZZUr)
3. [Combined Synthetic Train Set for 1 & 2 ](https://drive.google.com/open?id=1E5kI8CLoC-XffqQMTWwSpBIPp1Wb2tne)
4. [Transliteration (Transliterating Indic text to English)](http://workshop.colips.org/news2018/dataset.html)
5. [Translation](http://www.cfilt.iitb.ac.in/iitb_parallel/)

For other languages, download from relevant links of the works:

For Most Indian Languages:
- [Mann Ki Baat & Press Information Bureau Parallel  Corpora](https://www.aclweb.org/anthology/2020.lrec-1.462/)
- [PM India Speeches Parallel Text Corpora](https://arxiv.org/abs/2001.09907)

# WORKING
The task at hand at top level can be split into three major divisions 

- Text region detection

- Recognition of individual characters

- Natural Language Processing for translation/transliteration
