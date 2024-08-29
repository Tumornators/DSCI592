# DSCI592
Drexel University Master of Data Science Capstone II - 8/29/2024

Authors:

Joseph Novak - Drexel University Graduate Student, jn875@drexel.edu

Shawn Oyer - Drexel University Graduate Student, sbo33@drexel.edu

Patrick O'Brien - Drexel University Graduate Student, pjo44@drexel.edu

Thu Tran, Drexel University Graduate Student, tt537@dragons.drexel.edu

Abstract:

Lung cancer remains one of the deadliest cancers worldwide, with high mortality rates underscoring the urgent need for early and accurate diagnosis. In this study, we present a machine learning-based diagnostic toolset to discern healthy lung tissue from malignant tissue using computed tomography (CT) imagery. Our approach utilized two publicly available datasets: Iraq-Oncology Teaching Hospital/National Center for Cancer Diseases (IQ-OTH/NCCD) Lung Cancer dataset for model training/testing and the DLCTLungDetectNet dataset for validation. An image processing and UNET-based segmentation pipeline were developed, and two primary methodologies were evaluated: one utilizing raw and segmented lung scans fed into a Convolutional Neural Network (CNN), and another focusing on the extraction of texture features from segmented lung tissue for input into a Logistic Regression model. The CNN model trained on raw images exhibited near-perfect performance on the testing dataset but showed significant degradation in performance during external validation, suggesting overfitting and sensitivity to dataset differences. Conversely, the texture-based Logistic Regression model demonstrated more stable performance across both the testing and validation datasets, achieving the highest validation weighted F1 score of 80\%, highlighting its potential for broader application. Our findings reveal the critical importance of image segmentation and feature extraction techniques in developing reliable diagnostic tools for prediction of lung cancer.

Research Objectives: 

Specifically, this project aims at four research objectives:

1.Build a machine learning model(s) for accurate diagnosis of lung cancer from CT scans

2. Compare the effects of image segmentation and feature extraction on model(s) performance and benchmark against automated feature extraction in deep learning model(s)
   
3. Determine and visualize pixels/features highly impacting model(s) classification.
   
4. Assess the effectiveness of model(s) performance in an external validation setting.

Repository Contents:

1. CNN_Models.ipynb - Contains the code for all data pre-processing, model building, training, testing, validation, LIME heatmap, and all CNN model evaluation metrics
2. Lung_CT_ML_pipeline.ipynb -Contains the code for the feature extraction and model building, training, testing, validation, and all logistic regression model evaluation metrics
3. Image_Segmentation.ipynb - Contains the code for the skimage segmentation pipeline & UNET segmentation
4. UNET.ipynb - Contains the code for creating and training UNET model
5. README.md - Contains this README file
6. EDA.ipynb - Contains all of the Exploratory Data Analysis performed in this project

Stakeholders and Use:

Our motivations for this project are to provide an accurate, machine-learning based approach to accurately predicting/classifying malignant and non-malignant tissue from a given CT scan. The importance of early detection and accurate diagnosis play a critical role in improving patient outcomes that can lead to faster treatment along the disease timeline and improve the survival rate. This tool can ultimately support the entire healthcare industry by aiding healthcare doctors in reviewing CT scans as medical image classification tools are a valuable asset in all doctor's arsenals. In addition, the tool can support research scientists, who are constantly developing tools to be used for more accurate classification and predictions. Lastly, the tool can support actual patients and potentially improve their outcomes. This reinforces the significance of developing a successful and reliable model within the world of healthcare. 

Data Sources:

The first data source called the Iraq-Oncology Teaching Hospital/National Center for Cancer Diseases (IQ-OTH/NCCD) was used as a training and testing dataset that can be downloaded here: https://www.kaggle.com/datasets/hamdallak/the-iqothnccd-lung-cancer-dataset/data. The dataset is based on 110 cases collected in 2019 varying in gender, age, educational attainment, area of residence, and living status (AlYasriy et al., 2023). It contains 1102 images in JPG format divided into separate directories: Malignant, Benign, and Normal. 

The second data source called the DLCT Lung Detect Net was used as a validation dataset that can be downloaded here: https://www.kaggle.com/datasets/harshaldharpure/dlctlungdetectnet-lung-tumor-dataset. The dataset is a comprehensive and curated collection of diverse datasets related to lung tumors and pulmonary conditions (Dharpure, 2024). It contains 1000 images in JPG and PNG format divided into separate directories: Adenocarcinoma, Large Cell Carcinoma, Squamous Cell Carcinoma, and Normal.

Using the Scripts:

The extension of the scripts are all .ipynb files so they can be accessed and run within jupyter notebook and/or google collab as well as exported as a .py extension to import into any Python IDE.

License Use:

All data used were sourced from Kaggle and freely available under CC0 1.0 license. All of the code can be freely used as well.

References:

1. Al-Yasriy, Hamdalla, and Muayed Al-Huseiny. “The IQ-OTH/NCCD lung cancer dataset.” Kaggle, Mendeley Data, 2023, https://www.kaggle.com/datasets/hamdallak/the-iqothnccd-lung-cancer-dataset/data. Accessed 27 August 2024.

2. Dharpure, Harshal. “DLCTlUNGDetectNet - Lung Tumor Dataset.” Kaggle, Kaggle, 2024, https://www.kaggle.com/datasets/harshaldharpure/dlctlungdetectnet-lung-tumor-dataset. Accessed 27 August 2024.

3. Falk, Thorsten, et al. “U-NET: Deep Learning for Cell Counting, Detection, and Morpometry.” Research Gate, Nature Methods, January 2019, https://www.researchgate.net/publication/329716031_U-Net_deep_learning_for_cell_counting_detection_and_morphometry. Accessed 17 August 2024.

4. Ge, Yanqiu, et al. “Predicting post-stroke pneumonia using deep learning neural network approaches.” Pub Med, Int J Med Informatics, December 2019, https://pubmed.ncbi.nlm.nih.gov/31629312/. Accessed 17 August 2024.

5. Gobara, Mohamed. “Lung Cancer 98.8% Custom CNN Model.” Kaggle, Kaggle, January 2024, https://www.kaggle.com/code/mohamedgobara/lung-cancer-98-8-custom-cnn-model. Accessed 01 August 2024.

6. Naiborhu, Josua. “How to Interpret Black Box Models using LIME (Local Interpretable Model-Agnostic Explanations).” freeCodeCamp, 17 October 2022, https://www.freecodecamp.org/news/interpret-black-box-model-using-lime/. Accessed 28 August 2024.

7. National Cancer Institute. “Cancer of Any Site — Cancer Stat Facts.” SEER Cancer, National Cancer Institute, 2024, https://seer.cancer.gov/statfacts/html/all.html. Accessed 27 August 2024.

8. Shafi, Imran, et al. “An Effective Method for Lung Cancer Diagnosis from CT Scan Using Deep Learning-Based Support Vector Network.” NCBI, Cancers, 6 November 2022, https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9657078/. Accessed 29 August 2024.

9. Sprang, Maximilian, et al. “Batch effect detection and correction in RNA-seq data using machine-learning-based automated assessment of quality - BMC Bioinformatics.” BMC Bioinformatics, 14 July 2022, https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-022-04775-y. Accessed 19 August 2024.

10. Wright, George W., et al. “A Probabilistic Classification Tool for Genetic Subtypes of Diffuse Large B Cell Lymphoma with Therapeutic Implications.” Cancer Cell, vol. 37, no. 4, 2020, pp. 551-568. Cancer Cell, https://doi.org/10.1016/j.ccell.2020.03.015. Accessed 27 August 2024.
