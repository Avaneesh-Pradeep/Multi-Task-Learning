# Multi-Task-Learning

This project implements a multi-output Convolutional Neural Network (CNN) that simultaneously performs two related classification tasks: digit classification and color classification on a modified MNIST dataset. The model is built using the Keras Functional API.

---

## Objective
To train a single neural network to jointly perform:
- **Digit classification** (0–9)
- **Color classification** (grayscale vs color)

---

## Approach
- Constructed a CNN architecture with shared convolutional layers and two output heads
- Integrated **skip connections** (inspired by ResNet) to improve training stability
- Built a **custom Keras generator** to label and feed grayscale vs. RGB images dynamically along with digit labels
- Trained using categorical cross-entropy (digits) and binary cross-entropy (color), with equal loss weighting
- Monitored training performance with TensorBoard

---

##  Results
- Achieved **~98%** test accuracy on digit classification
- Achieved **~99%** test accuracy on color classification

---

## Acknowledgment
This project is based on a **guided project from Coursera**: *“Creating Multi-Task Models With Keras”*
All code was written, modified, and interpreted as part of hands-on learning and personal experimentation.

---

## Technologies
- Python
- TensorFlow / Keras
- NumPy, Matplotlib
- Jupyter / Google Colab
