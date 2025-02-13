# Real-Time Drowsiness Detection

This project implements a real-time drowsiness detection system using computer vision and deep learning. It utilizes a pre-trained model to classify eye states (open or closed) from webcam input and triggers an alert if drowsiness is detected.

## Table of Contents

- [Introduction](#introduction)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Real-Time Demo](#real-time-demo)
- [Dataset](#dataset)
- [Contributing](#contributing)


## Introduction

Drowsiness while driving is a major safety concern. This project aims to address this issue by providing a real-time drowsiness detection system. The system analyzes video frames from a webcam, detects faces and eyes, and uses a deep learning model to determine if the eyes are open or closed. If the system detects that the eyes are closed for a certain period, it triggers an audible alert to warn the user.

## Requirements

The project requires the following libraries:

- tensorflow
- opencv-python
- numpy
- matplotlib
- seaborn

## Installation

1. Clone the repository:

```bash
git clone https://github.com/oussemamansouri/Real-Time-Drowsiness-Detection.git
cd Real-Time-Drowsiness-Detection
```
2. Install the requirements :

You can install these using pip:

```bash
pip install -r requirements.txt
```

## Usage

**Model Training (Optional)**

If you want to train your own model, you can use the provided Jupyter Notebook (Eyes Classifier Model Training.ipynb).  The notebook covers data loading, preprocessing, model definition, training, and evaluation.  Run the cells in the notebook sequentially. Ensure you have the dataset prepared as described in the [Dataset](#dataset) section.

## Real-Time Demo

To run the real-time drowsiness detection demo use the provided Jupyter Notebook (Real Time Video Demo.ipynb). 

**The code :**

- Importing Required Libraries
- Load the trained model And Defining Class Labels
- Set sound frequency and duration
- Load Haarcascades for face and eyes (including eyeglasses)
- captures video from the webcam.
- Detects faces and eyes using OpenCV.
- Uses a deep learning model to classify eye state.
- Alerts the user if no face is detected for 3 seconds.
- Triggers a sleep alert if eyes are closed for too long.

## Dataset

The project uses a dataset of images of open and closed eyes. The code expects the dataset to be structured in a directory named MRL_DataSet/Test_dataset (adjust the path if needed).  Inside this directory, there should be subdirectories for each class (e.g., "Close-Eyes" and "Open-Eyes").  Each subdirectory should contain the images for that class.

**Dataset Source:**  The dataset used in this project is the [MRL Eye Dataset](https://www.kaggle.com/datasets/imadeddinedjerarda/mrl-eye-dataset).  This dataset contains images of eyes in various states and is suitable for training a drowsiness detection model.

You can download the dataset from the provided link.  The quality and quantity of the dataset significantly impact the model's performance.  If you use a different dataset, ensure it is properly structured and adjust the code accordingly.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request if you have any suggestions or improvements.