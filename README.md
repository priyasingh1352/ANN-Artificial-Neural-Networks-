# Artificial Neural Network (ANN) Project

## Overview

This project implements an **Artificial Neural Network (ANN)** using **TensorFlow** and **Keras** for predictive analysis and classification tasks.

The notebook demonstrates:

* Data preprocessing
* Building an ANN model
* Training and validation
* Model evaluation
* Prediction on new data

---

# Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* Jupyter Notebook

---

# Project Structure

```bash
├── ANN.ipynb              # Main Jupyter notebook
├── dataset.csv            # Dataset used for training
└── README.md              # Project documentation
```

---

# Artificial Neural Network Architecture

The ANN model contains:

1. Input Layer
2. Hidden Dense Layers
3. Output Layer

Features used in the model:

* ReLU activation function
* Sigmoid/Softmax output activation
* Adam optimizer
* Binary/Categorical Crossentropy loss

---

# Data Preprocessing

The following preprocessing steps are performed:

* Handling missing values
* Feature scaling
* Encoding categorical variables
* Train-test splitting

Libraries used:

```python
from sklearn.preprocessing import StandardScaler
from sklearn.model_selection import train_test_split
```

---

# Installation

Clone the repository:

```bash
git clone <your-github-repository-link>
cd <repository-name>
```

Install required packages:

```bash
pip install tensorflow keras pandas numpy matplotlib scikit-learn
```

---

# How to Run

1. Open Jupyter Notebook:

```bash
jupyter notebook
```

2. Open `ANN.ipynb`

3. Run all cells sequentially.

4. Train the model and evaluate results.

---

# Sample ANN Model Code

```python
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Dense

ann = Sequential()

ann.add(Dense(units=6, activation='relu'))
ann.add(Dense(units=6, activation='relu'))
ann.add(Dense(units=1, activation='sigmoid'))
```

---

# Model Training

The model is trained using:

```python
ann.fit(X_train, y_train, batch_size=32, epochs=100)
```

---

# Prediction

The ANN model predicts outputs based on input features and provides classification probabilities.

---

# Future Improvements

* Hyperparameter tuning
* Add Dropout layers to reduce overfitting
* Improve accuracy using deep learning optimization techniques
* Deploy the model using Flask or Streamlit

---

# Results

The project evaluates model performance using:

* Accuracy Score
* Confusion Matrix
* Loss and Accuracy Graphs

---

# Author

Priya Singh

---

# License

This project is licensed under the MIT License.
