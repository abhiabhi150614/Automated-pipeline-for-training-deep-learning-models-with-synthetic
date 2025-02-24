# Automated-pipeline-for-training-deep-learning-models-with-synthetic
It takes any classes which is required by users and genrate synthetic data for the classes and then train on the synthetic 
# Complete Image Classification Pipeline

This repository provides an end-to-end pipeline where the user only needs to supply the class names. The pipeline will:

1. **Generate Synthetic Images:**  
   Use the Gemini API to generate diverse image prompts based on user-defined class names, and then synthesize images using Stable Diffusion.

2. **Prepare YOLOv8 Dataset:**  
   Organize the generated images into a YOLOv8-compatible dataset format with train/validation splits and automatically create YOLO label files.

3. **Train YOLOv8 Model:**  
   Train a YOLOv8 model on the prepared dataset, and save the best model weights as `best.pt`.

---

## Features

- **Dynamic Prompt Generation:**  
  Generate detailed image descriptions for any class using the Gemini API.
  
- **Synthetic Image Generation:**  
  Create high-quality images using Stable Diffusion based on generated prompts.

- **Automated Dataset Preparation:**  
  Automatically split images into training and validation sets, and generate YOLOv8 label files.

- **End-to-End Training:**  
  Train a YOLOv8 model and output the best model weights for deployment.

---

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/your-repo.git
