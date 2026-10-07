# MNIST Handwritten Digit Classification using CNN

## Aim

The aim of this program is to build and train a **Convolutional Neural Network (CNN)** using TensorFlow/Keras to classify handwritten digits from the MNIST dataset. The model learns visual patterns from 28 × 28 grayscale images and predicts one of the ten digit classes (0–9).

## Dataset Used

The **MNIST (Modified National Institute of Standards and Technology) Handwritten Digit Dataset** is used.

- 60,000 training images
- 10,000 test images
- Image size: **28 × 28 pixels**
- Image type: **Grayscale**
- Number of classes: **10 (digits 0–9)**
- Pixel values are normalized from **0–255 to 0–1**

The dataset is loaded using `tensorflow.keras.datasets.mnist`.

## Model Used

A **Convolutional Neural Network (CNN)** is used for image classification. The model consists of:

- 3 Convolutional layers with ReLU activation
- 2 MaxPooling layers
- 1 Flatten layer
- 1 Dense layer with 64 neurons
- 1 Output layer with 10 neurons and softmax activation

The model is trained for **5 epochs** using the **Adam optimizer** and `sparse_categorical_crossentropy` loss function.

## Results

The model achieved a **test accuracy of approximately 99.34%** after 5 epochs.

The training accuracy improved from approximately **95.34% in the first epoch** to **99.34% in the fifth epoch**. The validation accuracy reached approximately **99.34%**.

The final training loss was approximately **0.0262**, while the validation loss was approximately **0.0262**.

Overall, the results show that the CNN performs very well on the MNIST handwritten digit classification task. The high validation accuracy and low loss indicate that the model has learned the digit patterns effectively and generalizes well to unseen images.
