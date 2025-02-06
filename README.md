# Real-Time License Plate Detection

A Python-based project for real-time license plate detection and character recognition using computer vision and machine learning techniques.

## Overview

This project implements an automated license plate recognition system that can:
- Detect license plates from video streams or images
- Segment individual characters from the detected plate
- Recognize the characters using a trained SVM model
- Output the complete license plate number

## Requirements

- Python 3.x
- OpenCV
- scikit-image
- scikit-learn
- numpy
- matplotlib
- imutils

## Project Structure


## How It Works

**1. License Plate Detection**
- Captures video frames or processes input images
- Converts images to grayscale and applies binary thresholding
- Detects potential license plate regions using dimensional analysis

**2. Character Segmentation**
- Extracts the license plate region
- Segments individual characters using connected component analysis
- Normalizes character images to 20x20 pixels

**3. Character Recognition**
- Uses a trained SVM model to recognize individual characters
- Combines predictions to form the complete license plate number
- Orders characters based on their position in the plate

## Model Training

The character recognition model is trained on a dataset of 20x20 pixel images containing:
- Numbers (0-9)
- Letters (A-Z, excluding I and O)
- 10 samples per character
- Linear SVM classifier with probability estimates

## Limitations

- Works best with clear, well-lit images
- May have reduced accuracy in poor lighting conditions
- Requires proper camera angle and distance for optimal results

## Contributing

Feel free to submit issues, fork the repository, and create pull requests for any improvements.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
