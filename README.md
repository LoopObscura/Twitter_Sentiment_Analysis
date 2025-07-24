# Image Classification Using Convolutional Neural Networks (CNN)

A convolutional neural network was developed to classify images of cats and dogs from a large dataset, achieving high accuracy by leveraging advanced deep learning techniques.

## Project Overview

The primary goal is to reliably differentiate between cat and dog images using a CNN, which excels at recognizing visual patterns and spatial hierarchies.

## Approach & Pipeline

- **Dataset:** 18,000 labeled images of cats and dogs.
- **Model Architecture:**
  - Convolutional layers (3x3 filters, batch normalization)
  - Feature map sizes: 32 → 64 → 96 → 96 → 64
  - Dense layers: 256 → 128 → 2 (output)
  - Dropout rates: 0.2 and 0.3 to reduce overfitting
- **Training Setup:**
  - 15 epochs
  - 80% training, 20% validation split
- **Preprocessing:**
  - Images were normalized and augmented for variability
  - Batch normalization and dropout to ensure robust generalization

## Results

- **Training Loss:** 0.0638  **Training Accuracy:** 97.59%
- **Validation Loss:** 0.3255 **Validation Accuracy:** 90.44%
- **Test Accuracy:** Between 97% and 99% on unseen test data

The results demonstrate that the model can accurately identify cats and dogs in new images, confirming its robustness and generalization capability.
