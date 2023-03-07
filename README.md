# CEST_MRI_Quantification


**This repository demonstartes some of my work in Image analysis using CEST MRI Images to quantify the parameters of small brain metabolites in brain that can provide important information about many neurodegenerative diseases, metabolic diseases, etc.**

Raw CEST Image consists of data at various saturation frequencies forming a Z- spectrum, which acts as an input to the model 

![image](https://user-images.githubusercontent.com/63582428/223332373-30ad3fe5-2409-426a-acfb-f1c12d5d6b78.png)

One of the traditional approaches to quantify the various parameters includes fitting a Lorentzian line-shape to the data, modeled as follows:

![image](https://user-images.githubusercontent.com/63582428/223332735-df92ad1a-f946-48c7-a7e7-4f44abf241c5.png)

There are many limitations with respect to this and other traditional approaches, time is a major factor.
Machine learning techniques can help reduce the time required tremenduosly

These Lorentzian parameters are used as ground truths for training the models.

This repository shows the use of a **CNN+LSTM** model to output these parameters (prediction of **amplitude of only amide pool** is shown in these demonstration)
