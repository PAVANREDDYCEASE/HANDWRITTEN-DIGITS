# HANDWRITTEN-DIGITS
# Handwritten Digits Recognition Using CNN

## Project Overview

This project implements a handwritten digit recognition system using Machine Learning and Deep Learning techniques.

The objective is to classify grayscale handwritten digit images into one of ten categories (0–9) using the MNIST dataset.

Six classification algorithms were developed and compared to identify the most effective model.

## Dataset

**Dataset:** MNIST Handwritten Digits Dataset

- Total images: 70,000
- Training images: 60,000
- Testing images: 10,000
- Image dimensions: 28 × 28 pixels
- Image type: Grayscale
- Classes: 0–9

The dataset is loaded using TensorFlow Keras.

## Models Implemented

### Traditional Machine Learning
1. K-Nearest Neighbors (KNN)
2. Support Vector Machine (SVM)
3. Logistic Regression
4. Random Forest

### Deep Learning
5. Artificial Neural Network (ANN)
6. Convolutional Neural Network (CNN)

## Model Comparison

All six models were compared using a common dataset containing 5,000 training samples and 1,000 validation samples.

| Model | Accuracy |
|---|---:|
| KNN | 92.60% |
| SVM | 94.40% |
| Logistic Regression | 89.00% |
| Random Forest | 93.20% |
| ANN | 92.60% |
| CNN | **95.30%** |

CNN achieved the highest accuracy in the controlled comparison.

## Final Model Performance

The selected full-data CNN was trained using 48,000 training images and evaluated on the official MNIST test dataset.

| Metric | Result |
|---|---:|
| Test Accuracy | **99.06%** |
| Test Loss | 0.04564 |
| Correct Predictions | 9,906 |
| Incorrect Predictions | 94 |

## CNN Architecture

- Input: 28 × 28 × 1
- Convolutional layer: 32 filters
- Max Pooling
- Convolutional layer: 64 filters
- Max Pooling
- Flatten layer
- Dense layer: 64 neurons
- Output layer: 10 neurons

**Optimizer:** Adam

**Loss Function:** Sparse Categorical Crossentropy

**Activation Functions:** ReLU and Softmax

## Technologies Used

- Python
- TensorFlow / Keras
- Scikit-learn
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## Project Structure

```text
Handwritten-Digits-Recognition/
│
├── handwritten_digits_recognition.ipynb
├── mnist_cnn_model.keras
├── README.md
├── requirements.txt
└── .gitignore
```

## Installation and Usage

### 1. Clone the repository

```bash
git clone https://github.com/PAVANREDDYCEASE/HANDWRITTEN-DIGITS.git
```

### 2. Navigate to the project directory

```bash
cd Handwritten-Digits-Recognition
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open the notebook

Open `handwritten_digits_recognition.ipynb` and execute the cells in order.

The MNIST dataset will be downloaded automatically through TensorFlow Keras when needed.

## Production Recommendation

CNN was selected as the final model because of its ability to learn spatial image features and its strong classification performance.

It achieved 99.06% accuracy on the official MNIST test dataset.

Further validation using real-world handwritten images is recommended before deployment.

## Future Enhancements

- Real-time handwritten digit recognition.
- Drawing-based digit recognition interface.
- Multi-digit number recognition.
- Model optimization and deployment.
- Testing with additional handwritten image datasets.

## Author

Developed as a Machine Learning and Deep Learning project focused on handwritten digit classification.
