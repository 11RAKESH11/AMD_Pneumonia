# AMD_Pneumonia
GPU-accelerated pneumonia detection using CNN models, optimized for AMD GPUs to enable fast and accurate medical image classification.

AMD GPU Accelerated Pneumonia Detection using CNN
Overview

Pneumonia is a serious respiratory disease that requires timely and accurate diagnosis. Traditional diagnostic methods rely on manual interpretation of chest X-ray images by radiologists, which can be time-consuming and subject to human error, especially in high-demand healthcare environments.

This project presents an automated pneumonia detection system using Convolutional Neural Networks (CNNs) to classify chest X-ray images into Pneumonia and Normal categories. The application is designed to support GPU acceleration, with a focus on AMD GPUs using ROCm, enabling faster training and efficient inference.

Key Features
Automated image classification using a CNN model
Support for GPU acceleration with AMD GPUs (ROCm compatibility)
Efficient processing of medical image data
Scalable design suitable for real-world applications
End-to-end workflow from training to prediction
Problem Statement

Manual analysis of chest X-ray images requires expertise and time. In many healthcare settings, especially in resource-constrained environments, there is a shortage of trained professionals. Additionally, CPU-based systems can be slow when processing large datasets, leading to delays in diagnosis.

Solution

This project uses a CNN-based deep learning model to automatically detect pneumonia from chest X-ray images. The system reduces reliance on manual interpretation and speeds up the diagnostic process. By leveraging GPU acceleration with AMD ROCm support, the model achieves improved performance and reduced training time.

AMD GPU Support

The application is designed to be compatible with AMD GPUs through ROCm (Radeon Open Compute platform). ROCm enables efficient parallel computation for deep learning workloads.

Supports GPU-based training and inference
Reduces computational time compared to CPU execution
Enhances scalability for large datasets

The code automatically utilizes available GPU resources when present.

Technologies Used
Python
TensorFlow / Keras
NumPy
Matplotlib
OpenCV
AMD ROCm (for GPU acceleration)
Project Structure
├── Pneumonia_Detection_AMD_GPU.ipynb
├── requirements.txt
└── README.md
Installation and Setup
1. Clone the Repository
git clone https://github.com/your-username/pneumonia-detection-amd-gpu.git
cd pneumonia-detection-amd-gpu
2. Install Dependencies
pip install -r requirements.txt
3. Run the Notebook
jupyter notebook
Model Training

The CNN model is trained on a dataset of chest X-ray images. The notebook includes steps for data preprocessing, model building, training, and evaluation. GPU support allows faster training when compatible hardware is available.

Prediction

The trained model can classify chest X-ray images into:

Pneumonia
Normal

A prediction function is included in the notebook for testing new images.

Results

The model achieves strong classification performance on the dataset. GPU acceleration helps reduce training time and improves overall efficiency compared to CPU-based execution.

Dataset

The dataset used for this project can be obtained from publicly available sources such as Kaggle chest X-ray datasets.

Conclusion

This project demonstrates the application of deep learning techniques in medical image analysis for pneumonia detection. By combining CNN-based classification with AMD GPU acceleration using ROCm, the system provides a fast, scalable, and efficient solution. It reduces dependency on manual diagnosis and enables quicker decision-making in healthcare settings. The approach highlights the potential of accessible GPU computing in building high-performance AI applications.

Future Work
Improve model accuracy using advanced architectures such as ResNet or EfficientNet
Develop a web-based interface for real-time predictions
Extend the system to detect multiple lung diseases
Integrate with clinical decision support systems
Note

The trained model file is not included due to size limitations. Users can train the model using the provided notebook.
