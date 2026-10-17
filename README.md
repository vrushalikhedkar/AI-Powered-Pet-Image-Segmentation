# AI Powered Pet Image Segmentation

A Deep Learning project that uses a Convolutional Neural Network (CNN) to segment pet images into foreground and background. The project provides a web interface built with Flask where users can upload cat or dog images and view the predicted segmentation mask.

## Project Overview

Image segmentation is a computer vision task that classifies pixels in an image to identify specific objects or regions. This project uses a CNN-based encoder-decoder architecture trained on the Oxford-IIIT Pet dataset to identify pet foreground regions.

## Features

- Upload cat and dog images through a web interface.
- Generate binary segmentation masks using a trained CNN model.
- Display the original image and predicted mask side by side.
- Process images using TensorFlow and Keras.
- Use a Flask application for interactive predictions.

## Technologies Used

- Python
- Deep Learning
- Convolutional Neural Networks (CNN)
- TensorFlow and Keras
- Flask
- NumPy
- Pillow
- HTML and CSS
- Oxford-IIIT Pet Dataset

## Project Structure

```text
AI-Powered-Pet-Image-Segmentation/
├── app.py
├── segmentation_model.h5
├── templates/
│   └── index.html
├── uploads/
└── README.md
```

The `uploads/` directory is created automatically when the Flask application starts.


## Model Details

- **Architecture:** CNN encoder-decoder
- **Input size:** 128 × 128 pixels
- **Input channels:** 3 (RGB)
- **Output:** Single-channel binary segmentation mask
- **Activation:** ReLU for hidden convolution layers and sigmoid for the output layer
- **Loss function:** Binary cross-entropy
- **Optimizer:** Adam

## Dataset

This project uses the Oxford-IIIT Pet dataset, which contains images of cats and dogs with corresponding segmentation annotations.

The model is trained to predict the pet foreground against the background.

## Limitations

- The model is designed for pet images, particularly cats and dogs.
- Predictions may contain inaccurate boundaries or incomplete regions.
- The model is a basic CNN encoder-decoder and may not perform as accurately as advanced segmentation architectures.
- The output is a binary mask, not a complete object-detection system.

## Future Improvements

- Improve segmentation accuracy through further training and evaluation.
- Add colored segmentation overlays to original images.
- Evaluate performance using IoU and Dice coefficient.
- Explore more advanced segmentation architectures.
- Deploy the application online.

## Author

Developed as a Deep Learning and Computer Vision portfolio project.
