# AI Super-Resolution with ESRGAN

This repository contains the implementation of an Enhanced Super-Resolution Generative Adversarial Network (ESRGAN) for image enhancement tasks.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project aims to enhance low-resolution images using deep learning techniques, specifically leveraging the power of ESRGAN. The model is trained on diverse datasets to improve image quality, making it suitable for various applications in image processing.

## Features

- **RRDBNet Architecture**: Includes the RRDBNet architecture, which consists of Residual in Residual Dense Blocks (RRDB) for robust feature extraction and enhancement.
- **Model Interpolation**: Ability to interpolate between PSNR and ESRGAN models to explore trade-offs in image quality.
- **Web Interface**: Integrates a Flask-based web application to upload images and receive enhanced outputs in real-time.

## Requirements

- Python 3.x
- PyTorch
- Flask
- OpenCV
- Other dependencies (specified in `requirements.txt`)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/your-repo.git
   cd your-repo
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

### Running the Web Application

1. Navigate to the repository directory.
2. Start the Flask app:
   ```bash
   python test.py
   ```
3. Open your browser and go to `http://localhost:5000` to access the application.
4. Upload an image and click 'Enhance' to see the output.

### Interpolating Models

To interpolate between PSNR and ESRGAN models, use the provided script `interpolate_models.py`:
```bash
python interpolate_models.py 0.5  # Replace with desired alpha value (0.0 to 1.0)
```

## File Structure

- `models/`: Contains pretrained models for PSNR and ESRGAN.
- `LR/`: Directory for low-resolution images used for testing.
- `test.py`: Flask web application for image enhancement.
- `interpolate_models.py`: Script to interpolate between PSNR and ESRGAN models.
- `README.md`: This file.

## Contributing

Contributions are welcome! Fork the repository and submit a pull request with your improvements.

## License

This project is licensed under the MIT License.

---
