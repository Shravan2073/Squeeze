

# Squeeze: Hybrid Medical Image Compression

## Project Description
**Squeeze** is a Flask-based web application designed for the high-efficiency compression of medical images, specifically targeting the DICOM format. This project employs a hybrid compression strategy that segments images into critical diagnostic "important" regions and non-critical background regions. 

By applying lossless techniques (Run-Length Encoding and Huffman Encoding) to important areas and lossy Discrete Cosine Transform (DCT) to the background, the application achieves significant file size reduction—targeting a compression ratio of 1.8 or higher—without compromising essential diagnostic details.

## Features
* **Target Compression Ratio**: 1.8x and higher while maintaining lossless quality for critical regions.
* **Hybrid Encoding Pipeline**: Combines automated Image Segmentation, Run-Length Encoding (RLE), Huffman Encoding, and Discrete Cosine Transform (DCT).
* **Medical Quality Standards**: Integrated validation for Peak Signal-to-Noise Ratio (PSNR) and Structural Similarity Index (SSIM).
* **Web Interface**: A streamlined Flask portal for secure image uploads and retrieval of compressed results.

## Documentation

### 1. Installation and Setup
Ensure you have Python 3.10+ installed. Install the necessary dependencies via the `requirements.txt` file:
```bash
pip install -r requirements.txt
```
Run applications 
```bash
uv run app.py
```
