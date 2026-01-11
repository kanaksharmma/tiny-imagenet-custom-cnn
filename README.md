📌 Tiny ImageNet Classification using Custom CNN
🔍 Project Overview

This project implements a custom Convolutional Neural Network (CNN) from scratch to perform image classification on the Tiny ImageNet dataset. The goal is to understand CNN architecture design, data handling for large-scale image datasets, and the complete deep learning workflow including training, evaluation, and result analysis.

The project is structured in a modular and notebook-driven manner to ensure clarity, reproducibility, and ease of understanding.

📂 Dataset Description
The project uses the Tiny ImageNet dataset, which is a smaller subset of the ImageNet dataset.
Number of classes: 200
Images per class: 500 training images
Image size: 64 × 64 RGB
Total training images: 100,000
Validation images: 10,000

Tiny ImageNet is widely used for benchmarking CNN architectures while keeping computational requirements manageable.
⚠️ Note: The dataset is not included in this repository due to size constraints. Instructions to download it are provided below.

🗂️ Repository Structure
tiny-imagenet-custom-cnn/
│
├── notebooks/
│   ├── 01_data_loading_and_exploration.ipynb
│   ├── 02_custom_cnn_model.ipynb
│   ├── 03_training_and_evaluation.ipynb
│   └── 04_final_evaluation_and_results.ipynb
│
├── src/
│   ├── __init__.py
│   └── models/
│       ├── __init__.py
│       └── custom_cnn.py
│
├── .gitignore
└── README.md

📘 Notebook Workflow
Notebook	Description
01_data_loading_and_exploration	Loads the Tiny ImageNet dataset, applies preprocessing, and performs basic data exploration
02_custom_cnn_model	Defines a custom CNN architecture using PyTorch
03_training_and_evaluation	Trains the CNN model and evaluates performance on validation data
04_final_evaluation_and_results	Analyzes final results, visualizes accuracy/loss curves, and provides observations

🧠 Model Architecture
Convolutional layers with ReLU activation
MaxPooling for spatial downsampling
Fully connected layers for classification
Softmax output over 200 classes

The model is implemented from scratch to strengthen understanding of CNN internals rather than relying on pretrained architectures.

⚙️ Training Details
Framework: PyTorch
Loss function: CrossEntropyLoss
Optimizer: Adam
Input size: 64 × 64 × 3
Evaluation metric: Classification accuracy

📊 Results & Observations
The model successfully learns discriminative features from the dataset.
Training and validation loss show stable convergence.
Certain visually similar classes exhibit confusion, highlighting the dataset’s complexity.
Performance can be further improved using data augmentation and deeper architectures.

▶️ How to Run the Project
Clone the repository:
git clone https://github.com/kanaksharmma/tiny-imagenet-custom-cnn.git
cd tiny-imagenet-custom-cnn

Download Tiny ImageNet dataset:
Official source: http://cs231n.stanford.edu/tiny-imagenet-200.zip

Extract it inside a data/ directory
Run notebooks in order:
notebooks/01 → 02 → 03 → 04

🚀 Future Improvements
Use data augmentation techniques
Experiment with deeper CNN architectures
Add batch normalization and dropout
Compare performance with pretrained models (ResNet, VGG)

👤 Author
Kanak Sharma
Artificial Intelligence & Machine Learning
Delhi,India
Artificial Intelligence & Machine Learning
Delhi, India
