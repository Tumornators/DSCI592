# DSCI592
Drexel University Master of Data Science Capstone II - 8/29/2024

Authors:

Joseph Novak - Drexel University Graduate Student, jn875@drexel.edu

Shawn Oyer - Drexel University Graduate Student, sbo33@drexel.edu

Patrick O'Brien - Drexel University Graduate Student, pjo44@drexel.edu

Thu Tran, Drexel University Graduate Student, tt537@dragons.drexel.edu

Abstract:

Here

Research Objectives: 

Specifically, this project aims at four research objectives:

1.Build a machine learning model(s) for accurate diagnosis of lung cancer from CT scans

2. Compare the effects of image segmentation and feature extraction on model(s) performance and benchmark against automated feature extraction in deep learning model(s)
   
3 . Determine and visualize pixels/features highly impacting model(s) classification.
   
4. Assess the effectiveness of model(s) performance in an external validation setting.

Repository Contents:

Stakeholders and Use:

Our motivations for this project are to provide an accurate, machine-learning based approach to accurately predicting/classifying malignant and non-malignant tissue from a given CT scan. The importance of early detection and accurate diagnosis play a critical role in improving patient outcomes that can lead to faster treatment along the disease timeline and improve the survival rate. This tool can ultimately support the entire healthcare industry by aiding healthcare doctors in reviewing CT scans as medical image classification tools are a valuable asset in all doctor's arsenals. In addition, the tool can support research scientists, who are constantly developing tools to be used for more accurate classification and predictions. Lastly, the tool can support actual patients and potentially improve their outcomes. This reinforces the significance of developing a successful and reliable model within the world of healthcare. 


Data Sources:

The first data source called the Iraq-Oncology Teaching Hospital/National Center for Cancer Diseases (IQ-OTH/NCCD) was used as a training and testing dataset that can be downloaded here: \href{https://www.kaggle.com/datasets/hamdallak/the-iqothnccd-lung-cancer-dataset/data}{IQ-OTH/NCCD download}. The dataset is based on 110 cases collected in 2019 varying in gender, age, educational attainment, area of residence, and living status \cite{AlYasriy2023}. It contains 1102 images in JPG format divided into separate directories: Malignant, Benign, and Normal. 

The second data source called the DLCT Lung Detect Net was used as a validation dataset that can be downloaded here: \href{https://www.kaggle.com/datasets/harshaldharpure/dlctlungdetectnet-lung-tumor-dataset}{DLCTLungDetectNet download}. The dataset is a comprehensive and curated collection of diverse datasets related to lung tumors and pulmonary conditions \cite{Dharpure2024}. It contains 1000 images in JPG and PNG format divided into separate directories: Adenocarcinoma, Large Cell Carcinoma, Squamous Cell Carcinoma, and Normal.

Using the Scripts:

The extension of the scripts are all .ipynb files so they can be accessed and run within jupyter notebook and/or google collab as well as exported as a .py extension to import into any Python IDE.

License Use:

All data used were sourced from Kaggle and freely available under CC0 1.0 license. All of the code can be freely used as well.

Sources:


