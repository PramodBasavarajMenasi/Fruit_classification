# 🍎 Fruit Classification using ResNet-18

## Overview
This repository contains the solution to the **Fruit Classification Kaggle Competition**. The task was to classify fruits into six categories: **fresh** and **rotten** states across three types of fruits. The model was built using the **ResNet-18** architecture, a pre-trained deep learning model, to classify the fruits. The project achieves an accuracy of **98%** on the test dataset.

---

## Dataset

The dataset consists of images of fruits that are categorized into six classes:
- **fresh_apple**
- **fresh_banana**
- **fresh_orange**
- **rotten_apple**
- **rotten_banana**
- **rotten_orange**

Each image represents a fruit in one of the two conditions: fresh or rotten. The goal is to train a model that can differentiate between fresh and rotten fruits across the three types: apple, banana, and orange.

The dataset is divided into:
- **Training Set**: Used to train the model.
- **Test Set**: Used to evaluate the model's performance after training.

---

## How I Built the Project

### 1. **Preprocessing the Data**:
   - The images were resized and normalized to the input size required for **ResNet-18**.
   - I used **data augmentation** techniques such as random rotations, zoom, and flipping to improve the model’s ability to generalize.
   
### 2. **Model Architecture**:
   - I used the **ResNet-18** model, pre-trained on the **ImageNet** dataset. This allows the model to leverage features learned from a large dataset to improve performance on the fruit classification task.
   - I fine-tuned the model by replacing the final classification layer to match the six classes in our dataset.
   
### 3. **Training the Model**:
   - I used the **Adam optimizer** with **cross-entropy loss** for training.
   - The model was trained for several epochs, and I monitored its performance using the **accuracy metric**.

### 4. **Evaluation**:
   - After training, I evaluated the model on the **test set** to check its accuracy.
   - The final accuracy achieved was **98%**, showing the model's ability to classify the fruits correctly.

---

## Results

The model achieved **98% accuracy** on the test dataset, which indicates that it successfully learned to distinguish between fresh and rotten fruits with a high level of precision. This model can be used in real-world applications like automated fruit sorting or quality control.

---

## How to Clone and Run the Project

### Cloning the GitHub Repository:
To clone the repository and get started, run the following command:

```bash
git clone https://github.com/PramodBasavarajMenasi/Fruit_classification.git/Fruit Classification.ipynb
```

### Running the Project on Google Colab:
You can run this project easily on Google Colab by clicking the following link:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1F3k-6fOUSzV-grNc5XJEAk1xg7ZaMguj?usp=sharing)