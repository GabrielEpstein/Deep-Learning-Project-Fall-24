# Deep-Learning-Project-Fall-24
This repository contains the code and accompanying resources for our Tulane University Introduction to Deep Learning project for the Fall 2024 semester.

By: Gabriel Epstein and Alex Motyka

---

## Introduction to Deep Learning Project Fall 2024

*This repository houses the code for our deep learning project focused on detecting tornadic supercells using Doppler radar data from the TorNET dataset. Our project explores the use of Convolutional Neural Networks (CNNs) and potentially Recurrent Neural Networks (RNNs) to identify tornado vortex signatures (TVS) based on radar velocity and reflectivity data. By Gabriel Epstein and Alex Motyka*

---

## Purpose:

The primary purpose of this project is to leverage deep learning techniques to predict tornadic events more accurately, with the hope of achieving or exceeding the detection performance of the National Weather Service (NWS). Early detection of tornadoes is crucial, as improving lead times by just a few minutes can significantly reduce fatalities. By utilizing the TorNET Doppler radar dataset, our project aims to build a model capable of identifying key radar signatures indicative of tornadic activity.

---

## Objective:

The goal of this project is to develop a deep learning model that can detect tornadic supercells based on Doppler radar images, specifically using velocity and reflectivity data. We aim to:
- Build a binary classification model (or multi-class if the problem is extended) to predict the presence or absence of tornado vortex signatures in radar data.
- Achieve comparable or improved detection performance compared to current models used by the NWS, which still require human validation.
- Explore different deep learning architectures, primarily CNNs, but also investigate the potential of using RNNs for sequential radar data.

---

## Data:

We are using the **TorNET Doppler radar dataset** that spans from 2013 to 2022. This dataset includes 10 years of radar data split across files ranging from 3 GB to 19 GB each, totaling over 150 GB. The dataset provides high-resolution Doppler radar products, including velocity and reflectivity readings, which are essential for detecting tornado vortex signatures.

- **Preprocessing**: Our preprocessing may involve techniques for noise reduction and data cleaning to handle the noisy nature of Doppler radar data.

---

## Challenges:

Some challenges we’re facing include:
- **Data Volume**: Handling over 150 GB of radar data efficiently while training deep learning models.
- **Data Noise**: Doppler radar data contains a significant amount of noise, potentially requiring substantial preprocessing.
- **Data Structure**: Each radar instance contains many additional measurements that may not be necessary for the model. We are working to figure out which data points are crucial for tornado detection and how to structure them for the model.

---

## Solution Overview:

Our solution involves creating a deep learning model that utilizes radar data to identify tornadoes. The project consists of the following key components:

1. **Data Loading and Preprocessing**:
   - Explore and structure Doppler radar data (velocity and reflectivity).
   - Apply noise reduction and prepare data for model input.

2. **Model Design**:
   - **Convolutional Neural Networks (CNNs)** will be used for feature extraction from radar images.
   - Potentially incorporate **Recurrent Neural Networks (RNNs)** to handle sequential radar data for more dynamic predictions over time.

3. **Training and Evaluation**:
   - Train the model using a split of the TorNET dataset, tuning hyperparameters to achieve optimal detection performance.
   - Evaluate the model using precision, recall, and other relevant metrics to ensure it can detect tornadoes with high accuracy.

4. **Challenges and Considerations**:
   - Extensive data preprocessing will be needed due to the noise and complexity of radar data.
   - We aim to reduce false positives and negatives to avoid unnecessary alerts, while maintaining high detection sensitivity.
