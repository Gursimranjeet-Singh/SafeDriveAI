# SafeDriveAI

SafeDriveAI is a real-time driver assistance system that features traffic sign recognition, lane detection, and collision detection.

## Project Overview
- **Traffic Sign Recognition**: Utilizes a CNN trained on the GTSRB dataset to identify traffic signs in real-time.
- **Lane Detection**: Detects lane lines using OpenCV with techniques like edge detection and line transformation.
- **Collision Detection**: Employs TensorFlow Hub's object detection models to detect and measure distances of objects.

---

## Installation

### 1. Set Up a Virtual Environment
```sh
python -m venv env
source env/bin/activate  # For Linux/macOS
env\Scripts\activate   # For Windows
```

### 2. Install Dependencies
```sh
pip install -r requirements.txt
```

### 3. Prepare Dataset
Download the GTSRB dataset and place it in the `data/GTSRB/` directory.

---

## How to Use

### Train the Model
Train the traffic sign recognition model using the provided dataset:
```sh
python -m src.train_model
```

### Start the System
Run the main script to activate all components:
```sh
python -m src.main
```
- Press `q` to exit.

---

## Features

### 1. Traffic Sign Recognition
- Recognizes traffic signs using a pre-trained CNN model.

### 2. Lane Detection
- Detects lane lines using OpenCV’s edge detection and line transformation.

### 3. Collision Detection
- Identifies objects and estimates distances with TensorFlow Hub’s detection models.

---

## Directory Structure
```
SafeDriveAI/
├── data/          # Contains the GTSRB dataset
├── models/        # Stores trained model files
├── src/           # Core scripts for functionalities
├── utils/         # Utility scripts for preprocessing and configurations
├── requirements.txt
└── README.md
```

---

## Dependencies
- TensorFlow & TensorFlow Hub
- OpenCV
- NumPy
- Pandas
- Scikit-learn

---

## Contributing
Contributions are welcome! Fork the repository, make changes, and submit a pull request.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

