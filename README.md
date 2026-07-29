# Image-Steganalysis-Using-DEEP-CNN
Image Steganalysis using Deep CNN (SRNet) developed as an MCA major project using PyTorch.
A deep learning pipeline for detecting hidden data (steganography) in digital images using SRNet — a CNN architecture purpose-built for steganalysis. The model learns subtle statistical noise-residual patterns to distinguish clean ("cover") images from images with covertly embedded data ("stego"), achieving 96% test accuracy on the BOSSBase 1.01 benchmark. Deployed through a Flask web interface for real-time cover/stego prediction.

**Key features:**
* End-to-end pipeline: data preprocessing → SRM noise-residual extraction → model training → evaluation → deployment
* Deep residual CNN (SRNet) trained with AdamW optimizer and cosine annealing LR scheduling
* Model evaluation on Accuracy, Precision, Recall, F1-score, and Confusion Matrix
* CrossEntropyLoss with label smoothing for improved generalization
* Flask web app for real-time image upload and cover/stego classification
* Dataset: BOSSBase 1.01 with LSB steganography embedding at 0.4 bits per pixel
