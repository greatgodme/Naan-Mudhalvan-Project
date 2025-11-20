
# Image Resolution Enhancer

This project demonstrates how to enhance the resolution of an image using a pre-trained model from TensorFlow Hub. The code downloads a low-resolution image, processes it, and improves its quality using Super Resolution techniques.

## Features
- Downloads an image from a URL.
- Preprocesses the image to make it compatible with the Super Resolution model.
- Upscales the image using a pre-trained ESRGAN model.
- Displays the original, low-resolution, and super-resolution images.
- Calculates PSNR (Peak Signal-to-Noise Ratio) to measure the quality of the enhanced image.

## Requirements

- TensorFlow 2.x
- TensorFlow Hub
- NumPy
- Matplotlib
- PIL (Python Imaging Library)
- Requests (for downloading the image)

Install the necessary libraries:
```bash
pip install tensorflow tensorflow_hub numpy matplotlib pillow requests
```

## How to Run

1. Clone the repository.
2. Run the script to download the image and process it using Super Resolution.
3. The script will display the original image, downscaled version, and the enhanced super-resolution image.

## Code Overview

- `preprocess_image(image_path)`: Prepares the image for model input.
- `save_image(image, filename)`: Saves the image tensor as a file.
- `plot_image(image, title)`: Displays the image.
- `downscale_image(image)`: Scales down the image to create a low-resolution version.
- The model used for Super Resolution is loaded from TensorFlow Hub.
- The PSNR is calculated to evaluate the quality of the super-resolution output.

## Example Output

The code will print out the time taken for processing and display both low-resolution and high-resolution images.
