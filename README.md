# Image Classification Project

This repository contains the code for an AI system designed to classify urban street images into three categories: **clean**, **littered**, and **with recycling bins (ecopoints)**. The project utilizes deep learning techniques, including transfer learning, to address the challenges posed by image variability in urban environments. This work aims to contribute to urban management and societal well-being through AI-powered image analysis.

---

## Project Overview

### Objectives
- Build a robust **Convolutional Neural Network (CNN)** for classifying urban images.
- Optimize model performance through hyperparameter tuning methods: **PSO (Particle Swarm Optimization)**, **Grid Search**, and **Random Search**.
- Enhance model accuracy using **transfer learning** with pre-trained networks.
- Assess model performance with classification metrics such as precision, recall, F1-score, and AUC.

### Motivation
Urban image classification is crucial for smart city management. This project focuses on developing an efficient AI solution to aid in environmental monitoring, specifically street cleanliness and recycling initiatives.

---

## Methodologies

### Implemented Strategies
1. **PSO (Particle Swarm Optimization):** A method for optimizing hyperparameters using a particle swarm approach.
2. **Random Search:** A stochastic method for hyperparameter tuning, exploring random combinations.
3. **Grid Search:** A thorough method that tests all possible combinations of hyperparameters.
4. **Simple Model:** A baseline model that uses the best-performing hyperparameters found through optimization.
5. **User-Specific Model:** A model designed for custom datasets and user-defined classifications.

### Dataset
- The project includes a **dataset** folder with subdirectories: `clean`, `litter`, and `recycle`. Each subdirectory contains 5 example images from the original dataset.
- The **original dataset** used for the project can be accessed on [Kaggle](https://www.kaggle.com/datasets/nw8vqlafd/dataset-ic).

---

## Code Structure

The code is organized into the following directories:

- **[models](#models):** Contains the trained models saved in `.h5` format.
  - **[Grid_SaveModel.h5](#models)**
  - **[PSO_SaveModel.h5](#models)**
  - **[Random_SaveModel.h5](#models)**
  - **[Simple_SaveModel.h5](#models)**

- **[results](#results):** Stores the performance results of the models, including performance metrics and classification outputs.
  - **[Grid_Excel.xlsx](#results)**
  - **[PSO](#results)**
  - **[Random](#results)**
  - **[Simple](#results)**

- **[src](#src):** Includes the Jupyter Notebooks for implementing the models and optimization techniques.
  - **[Grid.ipynb](#src)**
  - **[PSO](#src)**
  - **[Random](#src)**
  - **[Simple](#src)**

- **LICENSE:** Contains the project license file.
- **README.md:** This readme file providing an overview and project documentation.

---

## Data Processing and Model Architecture

1. **Image Preprocessing**
   - Images are resized to `224x224` pixels, normalized, and labeled using `LabelEncoder`.
   - The data is split into training and validation sets, ensuring balanced class distribution.

2. **Model Architecture**
   - **Base Model:** Pre-trained VGG16 network is used as the base for transfer learning.
   - **Custom Layers:** A series of layers including Flatten, Dropout, and Dense (Softmax activation for classification).
   - **Optimization:** Adam optimizer with sparse categorical cross-entropy loss.

3. **Training and Evaluation**
   - Models are trained on the training set and evaluated on the validation set.
   - Performance metrics include accuracy, confusion matrix, and classification reports.

4. **Hyperparameter Optimization**
   - **PSO, Grid Search, and Random Search** are applied to optimize learning rates and dropout rates.

5. **Results Storage**
   - The performance of each model is exported to **Excel files** for further analysis.
   - The trained models are saved in `.h5` format for later use.

---

## Results Analysis

### Optimization Techniques
- **Grid Search:** An exhaustive approach to hyperparameter tuning, resulting in visualized loss metrics.
- **Random Search:** A more efficient method for parameter optimization with competitive results.
- **PSO:** Adaptive optimization using the particle swarm algorithm, showing strong performance in fine-tuning.

### Model Evaluation
- All models, particularly the **Simple Model**, demonstrate high accuracy across the three categories (clean, littered, and recycling).
- The results are balanced across **precision**, **recall**, and **F1-score**, ensuring effective classification for real-world applications.
- Evaluation outputs include confusion matrices, classification reports, and performance graphs.

---

## Project Access

This repository serves as a code storage for the project and does not provide the dataset directly. For a more professional and functional view of the project, including access to the dataset, please refer to my Kaggle page:  
[Image Classification Project on Kaggle](https://www.kaggle.com/nw8vqlafd/dataset-ic)

---

### Notes
- Some code segments are written in **Portuguese (Portugal)**, as the project was developed using this language.

---

### Links to the Models, Results, and Code:

- [Models Folder](#models)
- [Results Folder](#results)
- [Source Code Folder](#src)
