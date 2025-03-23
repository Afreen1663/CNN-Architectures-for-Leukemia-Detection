# Leukemia Detection Using Deep Learning

This project leverages deep learning techniques, specifically CNN architectures, to detect leukemia and its subtypes from bone marrow images. The models used include ManualNet, DenseNet, LeNet, and VGGNet. Among them, **LeNet achieved the highest accuracy (96.7%) and is being used for the final implementation.**

The last phase of this project is to integrate the trained model into a **web-based platform**, which will allow medical professionals and patients to interact with the system for diagnosis and further information. This integration is currently in progress.

![Image](https://github.com/user-attachments/assets/c1cbb62c-ee00-4381-a5e8-6c91adc0d19c)

## Table of Contents
- [Project Overview](#project-overview)
- [CNN Architectures Used](#cnn-architectures-used)
  - [LeNet (Highest Accuracy)](#lenet-highest-accuracy)
  - [ManualNet](#manualnet)
  - [DenseNet](#densenet)
  - [VGGNet](#vggnet)
- [Web Integration (Upcoming Phase)](#web-integration-upcoming-phase)
- [Dataset](#dataset)
- [Installation & Usage](#installation--usage)
- [Results](#results)
- [Future Improvements](#future-improvements)

## Project Overview
Leukemia is a type of blood cancer that affects white blood cells. Early and accurate detection is crucial for effective treatment. This project applies deep learning techniques to analyze bone marrow images and identify leukemia along with its subtypes.

![Image](https://github.com/user-attachments/assets/1a5e80fe-cd6e-4957-9f41-3e400f565a9f)

### Goals:
- Train CNN models to detect leukemia and classify its subtypes.
- Identify the most accurate architecture for deployment.
- Develop a web-based system for doctors and patients to use.

## CNN Architectures Used
Several CNN models were trained and evaluated for leukemia detection. Below are their details and performance results:

### LeNet (Highest Accuracy)
LeNet achieved the **highest accuracy (96.7%)**, making it the best candidate for deployment in the web-based platform.
- **Layers:**
  - Convolutional Layers: 2
  - Pooling Layers: 2
  - Fully Connected Layers: 2
- **Activation Functions:** ReLU, Softmax
- **Optimizer:** Adam
- **Loss Function:** Categorical Crossentropy

<img width="751" alt="Image" src="https://github.com/user-attachments/assets/7b3f291e-8de1-4ff5-a349-5779fdf21976" />

### ManualNet
ManualNet was designed as a lightweight CNN for faster processing.
- **Accuracy:** 93.8%
- **Layers:**
  - Convolutional Layers: 1
  - Pooling Layers: 1
  - Fully Connected Layers: 2
- **Optimizer:** RMSprop

### DenseNet
DenseNet is a deep architecture that improves feature propagation.
- **Accuracy:** 38.7%
- **Unique Feature:** Dense connectivity between layers
- **Optimizer:** Adam
- **Loss Function:** Categorical Crossentropy

### VGGNet
VGGNet is a widely used deep CNN architecture.
- **Accuracy:** 54.5%
- **Pretrained Model:** VGG16 (ImageNet weights)
- **Additional Layers:** Fully connected layers for classification
- **Optimizer:** Adam
- **Loss Function:** Categorical Crossentropy

## Web Integration (Upcoming Phase)
The final step of this project is to integrate the trained LeNet model into a **web application** where:
- **Patients** can check their diagnosis, treatments, causes, and other details.
- **Doctors** can upload bone marrow images to detect leukemia and its subtypes.

This phase is currently in development.

## Dataset
- The dataset consists of bone marrow images categorized into different leukemia subtypes.
- Images were preprocessed and augmented for better model generalization.

<img width="746" alt="Image" src="https://github.com/user-attachments/assets/6b7cf46d-6a10-4ee3-b733-35905c31dca0" />

## Installation & Usage
### Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/Afreen1663/CNN-Architectures-for-Leukemia-Detection.git
   ```
2. Install dependencies:
   ```sh
   pip install tensorflow keras numpy opencv-python matplotlib flask
   ```

### Running the Model
1. Execute the Jupyter notebooks to train models.
2. Load a trained model and use it for predictions.

### Running the Web App (Upcoming Feature)
Once integration is completed, run:
```sh
python app.py
```

## Results
- **LeNet achieved the highest accuracy (96.7%)** and will be used in the final deployment.
- The trained models successfully classify leukemia subtypes with high precision.

## Future Improvements
- Complete web integration for real-world usability.
- Improve accuracy by experimenting with newer architectures.
- Deploy as a cloud-based service for remote access.
