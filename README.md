# Image Classification Project

Welcome to the **Image Classification Project**! This repository contains the code and documentation for classifying urban street images into three categories: **clean**, **littered**, and **with recycling bins (ecopoints)**. The project leverages deep learning techniques, including transfer learning, and various hyperparameter optimization methods to achieve efficient classification.

---

## Project Overview

This project aims to build a robust AI system for classifying urban street images. The focus is on detecting the cleanliness of streets and identifying the presence of recycling bins. The models were trained using a custom dataset, and hyperparameter optimization was applied to improve the models' performance.

---

## Project Access

This repository serves as a code storage for the project. For a more professional and functional view, including access to the full dataset, please visit the project on [Kaggle](https://www.kaggle.com/nw8vqlafd).

---

## Language Note

**Important**: Some sections of the code and documentation are written in **Portuguese (Portugal)**, as the project was initially developed in that language. However, this repository is structured for ease of use, with all key information available in English.

---

# Dataset

The project includes a **dataset** folder that serves as an example of the original dataset used. The dataset is divided into three subfolders:

- **clean**: Images of clean streets.
  <br><img src="dataset/clean/Clean_0054.png" alt="Clean Street Example" width="200"/>
- **litter**: Images of streets with litter.
  <br><img src="dataset/litter/Litter_0073.png" alt="Littered Street Example" width="200"/>
- **recycle**: Images of streets with recycling bins (ecopoints).
  <br><img src="dataset/recycle/Ecoponto_0033.png" alt="Recycle Bin Example" width="200"/>

Each folder contains 5 example images to illustrate the original dataset. For the complete dataset, you can access it on [Kaggle](https://www.kaggle.com/datasets/nw8vqlafd/dataset-ic).

---

## Repository Structure

This repository is organized into the following sections:

### **1. Models (`models/`)**
Contains the trained models saved in `.h5` format. These models were used to classify images into the respective categories:
- **`Grid_SaveModel.h5`**: Model optimized using Grid Search.
- **`PSO_SaveModel.h5`**: Model optimized using Particle Swarm Optimization (PSO).
- **`Random_SaveModel.h5`**: Model optimized using Random Search.
- **`Simple_SaveModel.h5`**: Baseline model without optimization.

### **2. Results (`results/`)**
Holds the performance metrics and results of the models:
- **`Grid_Excel.xlsx`**: Results from the Grid Search optimization.
- **`PSO`**: Results from the PSO optimization.
- **`Random`**: Results from the Random Search optimization.
- **`Simple`**: Results from the baseline model.

### **3. Source Code (`src/`)**
Includes the Jupyter Notebooks and scripts for training the models and performing hyperparameter optimization:
- **`Grid.ipynb`**: Script for training the model with Grid Search optimization.
- **`PSO`**: Script for training the model with PSO optimization.
- **`Random`**: Script for training the model with Random Search optimization.
- **`Simple`**: Script for training the baseline model.

### **4. License (`LICENSE`)**
Contains the license file for the project.

### **5. Documentation (`README.md`)**
This readme file, which provides an overview of the project.

---

## License

This project is licensed under the [MIT License](/LICENSE). Feel free to use, modify, and distribute this project.

---

## Contact

For any questions or suggestions, please contact:
- **GitHub**: [LHTravassos](https://github.com/LHTravassos)
