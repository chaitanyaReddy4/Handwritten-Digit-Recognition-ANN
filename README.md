# Handwritten Digit Recognition using ANN

## Project Overview

This project implements a Deep Learning model using an Artificial Neural Network (ANN) to recognize handwritten digits from 0 to 9.

The model is trained and evaluated using the MNIST dataset, which contains 70,000 grayscale images of handwritten digits. TensorFlow and Keras are used to build, train and evaluate the neural network.

## Dataset

- **Dataset:** MNIST Handwritten Digits
- **Total Images:** 70,000
- **Training Images:** 60,000
- **Testing Images:** 10,000
- **Image Dimensions:** 28 × 28 pixels
- **Classes:** 10 (Digits 0–9)

The dataset is automatically downloaded through TensorFlow Keras.

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Pandas
- Scikit-learn
- Seaborn
- Jupyter Notebook

## Project Workflow

1. Loaded the MNIST dataset using TensorFlow Keras.
2. Explored the training and testing datasets.
3. Visualized handwritten digit images using Matplotlib.
4. Normalized pixel values from 0–255 to 0–1.
5. Built an ANN using Flatten and Dense layers.
6. Compiled the model using Adam optimizer and Sparse Categorical Crossentropy loss.
7. Trained the model using different epochs and batch sizes.
8. Evaluated performance using accuracy and loss.
9. Generated accuracy and loss graphs.
10. Analyzed predictions using a confusion matrix and classification report.
11. Saved the trained ANN models.

## ANN Architecture

The neural network consists of the following layers:

| Layer | Configuration |
|---|---|
| Input | 28 × 28 pixels |
| Flatten | 784 features |
| Hidden Layer 1 | 128 neurons, ReLU |
| Hidden Layer 2 | 64 neurons, ReLU |
| Output Layer | 10 neurons, Softmax |

**Total Trainable Parameters:** 109,386

## Model Configuration

- **Optimizer:** Adam
- **Loss Function:** Sparse Categorical Crossentropy
- **Evaluation Metric:** Accuracy
- **Best Epochs:** 10
- **Best Batch Size:** 64

## Experimental Results

Different training configurations were tested to compare model performance.

| Epochs | Batch Size | Test Accuracy | Test Loss |
|---|---|---|---|
| 5 | 32 | 97.59% | 0.0887 |
| 10 | 32 | 97.38% | 0.1146 |
| 10 | 64 | 97.84% | 0.0832 |

**Best Result:**
- Test Accuracy: 97.84%
- Test Loss: 0.0832
- Epochs: 10
- Batch Size: 64

The classification report also achieved approximately 98% weighted precision, recall and F1-score with the original trained model.

## Model Evaluation

The model was evaluated using:

- Training and validation accuracy.
- Training and validation loss.
- Test accuracy and test loss.
- Confusion Matrix.
- Precision, Recall and F1-score.
- Individual digit predictions.

## Project Structure

```text
Handwritten_Digit_Recognition/
│
├── digit_recognition.ipynb
├── mnist_ann_model.keras
├── mnist_ann_model_best.keras
└── README.md
```

## Installation and Execution

**1. Clone the repository**

```bash
git clone <your-repository-url>
```

**2. Navigate to the project folder**

```bash
cd Handwritten_Digit_Recognition
```

**3. Install the required libraries**

```bash
pip install tensorflow numpy matplotlib pandas scikit-learn seaborn pillow jupyter
```

**4. Launch Jupyter Notebook**

```bash
jupyter notebook
```

**5. Open and execute**

Open `digit_recognition.ipynb` and execute the notebook cells sequentially.

## Conclusion

The project successfully demonstrates handwritten digit classification using an Artificial Neural Network.

The best experimental configuration achieved 97.84% test accuracy on the MNIST dataset. The project demonstrates the application of Deep Learning, image preprocessing, neural network training and model evaluation for image classification tasks.
