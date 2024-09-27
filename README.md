# Deep Art: Universal Style Transfer with Deep Learning

This project implements **Deep Art**, an advanced neural style transfer technique utilizing **Whitening and Coloring Transform (WCT)** for real-time, high-quality artistic stylization of images. By leveraging deep learning techniques with TensorFlow and Keras, users can apply the artistic style of any image to another content image, producing stunning results with minimal latency.

Unlike traditional methods, **Deep Art** is designed for universal style transfer, meaning it does not require style images during model training. This allows it to apply styles between arbitrary content and style images using a WCT-based pipeline, delivering superior quality while reducing memory consumption.

## Key Features

- **Universal Style Transfer**: Apply artistic styles from any source image to any content image.
- **Whitening and Coloring Transform (WCT)**: A fast, efficient technique for image stylization.
- **Real-Time Processing**: Supports real-time style transfer on images and videos.
- **Multi-Level Stylization Pipeline**: Uses multiple layers of VGG19 for style transfer, creating deeper artistic effects.
- **Easy-to-Use Interface**: Command-line interface (CLI) and extendable for web or mobile applications.
- **Webcam Integration**: Real-time style transfer using a webcam feed.

## Demo

Example outputs of style transfer:

<p align="center">
  <img src="samples/original_image.jpg" width="300px" alt="Original Image">
  <img src="samples/stylized_image.jpg" width="300px" alt="Stylized Image">
  <img src="https://github.com/1216-dev/Deep-Art/blob/main/input.png" width="300px" alt="Another Stylized Output">
</p>

## Getting Started

Follow these instructions to set up the project on your local machine.

### Prerequisites

Ensure that you have the following dependencies installed:

- Python 3.x
- TensorFlow >= 2.x
- Keras >= 2.4
- OpenCV (for real-time webcam feed)
- NumPy

### Installation

1. Clone this repository:

    ```bash
    git clone https://github.com/YourUsername/Deep-Art.git
    cd Deep-Art
    ```

2. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

3. Download pre-trained VGG19 model weights (if applicable):

    ```bash
    # Add the script or instructions for downloading model weights
    ./scripts/download_models.sh
    ```

### Usage

#### Image Stylization

To apply style transfer to an image:

```bash
python stylize.py --content_path path/to/content.jpg --style_path path/to/style.jpg --output_path path/to/output.jpg
