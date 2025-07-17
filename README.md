Anvesha AI – AI-Powered Hope for Finding the Missing

Anvesha AI is a computer vision project focused on identifying and locating missing children from real-world images using facial recognition powered by AI. By combining Haar-Cascade-based face detection and a CNN-based classifier, the system can scan through images and highlight those that contain children. The core goal of this project is to support social good by helping communities and authorities detect missing individuals in visual data.

🚀 Features

Face detection using Haar-Cascade classifiers

CNN model for child face classification

Image classification and filtering

Modular design for easy testing and extension

📂 Project Structure

├── dataset/               # Contains raw and processed image datasets
├── step-1-cnn/            # CNN model training scripts and model outputs
├── step-2-haarcascade/    # Face detection test scripts (optional)
├── step-3-final/          # Final integrated face detection + classification pipeline
├── requirements.txt       # Required Python packages
├── README.md              # Project documentation (this file)

📸 *Datasets Used*

Large Age-Gap Face Verification

KinFaceW

*After preprocessing:*

2,168 child face images

2,587 adult face images

All resized to 150x150 pixels and converted to grayscale.

python main.py

*How to Run:*

1. Train CNN

$ cd step-1-cnn
$

2. (Optional) Evaluate Haar-Cascade accuracy

$ cd step-2-haarcascade
$ python main.py

3. Run Final Pipeline

# Copy best model from step-1-cnn to step-3-final/model/
$ cd step-3-final
$ python main.py
