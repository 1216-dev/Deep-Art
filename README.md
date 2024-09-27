#Deep Art: Universal Style Transfer with Deep Learning


This project implements Deep Art, an advanced neural style transfer technique, utilizing Whitening and Coloring Transform (WCT) for real-time and high-quality artistic stylization of images. By leveraging deep learning techniques with TensorFlow and Keras, it allows users to apply the artistic style of one image to any content image, creating beautiful results with minimal latency.

Unlike traditional methods, Deep Art is designed for universal style transfer, meaning no style images are needed for model training. It can transfer styles between any arbitrary content and style images through a WCT-based pipeline, delivering superior quality while reducing memory usage.

Key Features
Universal Style Transfer: Transfer artistic styles from any source image to any content image.
Whitening and Coloring Transform (WCT): A fast, efficient technique for stylization.
Real-Time Processing: Apply style transfer on images or videos in real-time.
Multi-Level Stylization Pipeline: Uses multi-layer reconstruction to enhance the artistic effect.
Easy-to-Use Interface: Includes CLI and can be extended for use with web or mobile applications.
Webcam Integration: Real-time style transfer through webcam feed.
Demo
You can see some example outputs below:

<p align="center"> <img src="samples/original_image.jpg" width="300px"> <img src="samples/stylized_image.jpg" width="300px"> </p>
Getting Started
Prerequisites
To get started with Deep Art, ensure that you have the following dependencies installed:

Python 3.x
TensorFlow >= 2.x
Keras >= 2.4
OpenCV (for real-time webcam feed)
NumPy
