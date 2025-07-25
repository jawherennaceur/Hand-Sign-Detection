# Maze Image Classification with MobileNetV2

This project trains a Convolutional Neural Network using MobileNetV2 with transfer learning to classify images from a custom dataset . It also includes webcam image capture and real-time prediction using Google Colab.

---

## Project Structure

- **Model**: MobileNetV2 with custom classification head  
- **Framework**: TensorFlow + Keras  
- **Dataset**: Two-class image folder structure  
- **Data Augmentation**: Applied using `ImageDataGenerator`  
- **Training Platform**: Google Colab  
- **Image Capture**: JavaScript + Colab + OpenCV integration  

---

## Setup

1. Mount Google Drive
2. Copy the dataset folder `data` to `/content`
3. Structure:
    ```
    data/
    ├── fist/
    └── palm/
    ```

---

## Dependencies

```bash
tensorflow
opencv-python
matplotlib
scikit-learn
scikit-image
Pillow
```

---

## Training

- Image resolution: 224x224  
- Batch size: 10  
- Loss: categorical_crossentropy  
- Optimizer: Adam (lr=0.00008)  
- Callbacks: Custom accuracy-based early stopping (optional)  
- Augmentations:
  - Rotation, shift, zoom, flip, brightness

---

## Sample Training Log

- Train Accuracy: ~100%
- Validation Accuracy: ~96–100%
- Model saved as `need_help.h5`

---

## Webcam Prediction

- Captures an image from your webcam in Google Colab
- Converts to RGB format
- Resizes to 224x224
- Normalizes pixel values
- Runs prediction with trained model

---
