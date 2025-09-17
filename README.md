# Credit Card Optical Character Recognition

A Python-based OCR system that uses OpenCV and Pytesseract to detect and extract credit card numbers and cardholder information from credit card images.

## Overview

This repository contains a complete implementation of an optical character recognition (OCR) pipeline specifically designed for credit card text extraction. The system processes credit card images to identify and extract:

- Credit card numbers
- Cardholder names
- Other relevant text information

## Features

- OpenCV-based image preprocessing
- Pytesseract OCR integration
- Jupyter notebook with step-by-step implementation
- Comprehensive image dataset for testing
- Custom utility functions for image processing

## Sample Output

![feature_image1](https://user-images.githubusercontent.com/8759492/150893179-988ed159-fa72-4ed2-a74f-8bd86f8dccc7.png)
![cccorrect2](https://user-images.githubusercontent.com/8759492/150893195-775a1a9d-27a3-462e-bbfc-049850278ff1.png)
![cccorrect3](https://user-images.githubusercontent.com/8759492/150893207-5ecc5671-a0cb-47b7-8b46-87d88840ce34.png)

## Getting Started

### Prerequisites

- Python 3.6+
- OpenCV
- Pytesseract
- Jupyter Notebook
- Required Python packages (see notebook for full list)

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd CreditCard_Optical_Character_Recognition
```

2. Install required dependencies:
```bash
pip install opencv-python pytesseract jupyter numpy pandas matplotlib seaborn scikit-learn torch torchvision
```

### Usage

1. **Jupyter Notebook**: Open `notebooks/Credit_Card_Reader_Implementation.ipynb` and follow the step-by-step instructions
2. **Image Dataset**: Explore the sample images in the `/images` folder
3. **Custom Implementation**: Use the utility functions in `scripts/utils2.py` for your own implementations

### Docker Usage

To run this project using Docker:

1. **Build the Docker image**:
```bash
docker build -t credit-card-ocr .
```

2. **Run the container**:
```bash
docker run -it --rm -p 8888:8888 -v $(pwd):/workspace credit-card-ocr
```

3. **Access Jupyter Notebook**:
   - Open your browser and navigate to `http://localhost:8888`
   - Use the token provided in the terminal output

## Project Structure

```
CreditCard_Optical_Character_Recognition/
├── images/                    # Sample credit card images
├── notebooks/                 # Jupyter notebook implementation
├── scripts/                   # Utility functions
├── README.md                  # This file
├── objectives.md             # Project objectives and goals
└── .gitignore               # Git ignore file
```

## Additional Resources

- [Implementation Blog Post](https://philippeheitzmann.com/2022/01/implementing-vgg19-and-custom-built-style-transfer-algorithms-to-artificially-stylize-images/) - Detailed implementation walkthrough
- [Project Objectives](objectives.md) - Project goals and objectives

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).
