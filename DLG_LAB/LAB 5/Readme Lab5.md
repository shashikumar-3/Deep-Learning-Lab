## Handwritten Digit Recognition with an RNN (LSTM)

### Aim
The goal of this project is to build and train a Recurrent Neural Network (specifically an LSTM) to classify handwritten digits from images by treating each image as a sequence of pixel rows over time.

### Dataset
- **Name:** MNIST Dataset
- **Input:** 60,000 training images and 10,000 test images of $28 \times 28$ grayscale pixels.
- **Preprocessing:** Rescaled pixel values to range $[0, 1]$, reshaped inputs to shape `(samples, 28, 28)`, and one-hot encoded the 10 target digit classes.

### Model Architecture
- **LSTM Layer:** 128 hidden units with standard `relu` activation (can be swapped with `tanh`), taking an input shape of `(28, 28)` representing 28 timesteps of 28 features each.
- **Dense Layer:** 10 output units with `softmax` activation to generate multiclass class probabilities.

### Results
- **Final Test Accuracy:** **~98.56%** achieved in 10 epochs using the Adam optimizer and categorical cross-entropy loss.