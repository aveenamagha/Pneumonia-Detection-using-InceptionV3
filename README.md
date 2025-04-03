# Pneumonia-Detection-using-InceptionV3

# Project Overview

This project classifies chest X-ray images as NORMAL or PNEUMONIA using InceptionV3, a deep learning model. The model is fine-tuned to enhance automated pneumonia detection from medical imaging, improving accuracy in diagnosing lung infections.

# Dataset

The dataset consists of chest X-ray images categorized into:

NORMAL – Healthy lung X-rays.

PNEUMONIA – X-rays showing signs of pneumonia.

🔗 Dataset Link:  https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

# Dataset Distribution

Training Set: 5216 images

Validation Set: 16 images

Test Set: 624 images

# Preprocessing & Augmentation

Images resized to 224×224×3 (RGB format) for model compatibility.

Applied augmentation techniques like rotation, flipping, and zooming.

Pixel values normalized to 0-1 range for stable training.

# Model Architecture

Base Model: InceptionV3 (pretrained on ImageNet).

Added Layers:

Global Average Pooling

Dense Layer (128 neurons, ReLU activation)

Dropout Layer (0.5)

Output Layer (1 neuron, Sigmoid activation)

# Fine-Tuning: Last 100 layers of InceptionV3 were unfrozen and retrained.

# Training & Evaluation

Optimizer: Adam (learning rate: 1e-5)

Loss Function: Binary Crossentropy

Early Stopping: Enabled (patience: 5 epochs)

Epochs: 20

# Training Results

Training Accuracy	     98.88%	 

Validation Accuracy     100%
  
# Test Results

Test Accuracy: 91.03%

Test Loss: 0.2280

# Sample Image Prediction

A test image was selected and processed.

The model correctly classified it as NORMAL, confirming its reliability.

# Key Takeaways

✅ High Accuracy: Achieved 91.03% test accuracy.
✅ Effective Fine-Tuning: Model improved through selective training.
✅ Real-World Applicability: The model successfully identified pneumonia cases.

How to Use

model link : https://drive.google.com/file/d/1-AdxGtKpkaxwyZdF12YJ3dpjpnCkrQ3B/view?usp=drive_link

1️⃣ Install Dependencies

Ensure TensorFlow and required libraries are installed.

2️⃣ Load & Train the Model

Train using the provided dataset and parameters.

3️⃣ Evaluate Performance

Run evaluation on the test dataset to check accuracy.

4️⃣ Make Predictions

Input a chest X-ray to classify it as NORMAL or PNEUMONIA.

# Contact
For questions or improvements, feel free to reach out!

📧 Email: aveenamagham2003@gmail.com
