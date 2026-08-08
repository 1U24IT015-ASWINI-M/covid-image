# covid-image
COVID-19 Image Classification Using CNN
Project Overview

The COVID-19 Image Classification project is a deep learning-based image classification system developed to identify whether a chest X-ray image belongs to a COVID-19 positive patient or a Normal patient. The main purpose of this project is to support faster and more accessible COVID-19 detection using Artificial Intelligence.

The project uses Convolutional Neural Networks (CNN) to automatically learn important visual features from chest X-ray images and classify them into two categories: COVID-19 and Normal. The dataset contains 251 chest X-ray images, where each image is resized to 128 × 128 pixels with 3 color channels (RGB). The image data is stored in CovidImages.npy, while the corresponding class labels are stored in CovidLabels.csv.

Technologies Used
Python
TensorFlow / Keras
CNN (Convolutional Neural Network)
NumPy
Pandas
OpenCV
Matplotlib
Seaborn
Scikit-learn
Google Colab
Project Workflow

Chest X-ray Images → Data Preprocessing → Label Encoding → Train/Validation/Test Split → CNN Model Training → Model Evaluation → COVID/Normal Prediction

Two CNN architectures were developed and compared. The first model used 3 convolutional layers, while the second model used a simpler 2-convolutional-layer architecture to reduce complexity and improve generalization. The final selected model consisted of convolution, max-pooling, flatten, dense and sigmoid output layers.

Model Performance

The final 2-layer CNN model was selected because it provided strong performance with a simpler architecture. The project evaluation recorded:

Training Accuracy: 99.43%
Validation Accuracy: 100%
Training COVID Recall: 98.70%
Validation COVID Recall: 100%
Test Accuracy: 100%
Test COVID Recall: 100%

Note: The notebook contains a later written observation reporting different test metrics (97.37% accuracy and 94.12% COVID recall), which does not match the actual printed test output above. For your project presentation, it is safer to mention the actual executed test output unless you intentionally revise the notebook.

Conclusion

The project successfully demonstrates how CNN-based deep learning can be applied to chest X-ray image classification for COVID-19 detection. The system provides a rapid and non-invasive diagnostic aid and can potentially support healthcare professionals. A key future improvement is to use a larger and more diverse dataset to improve robustness and generalization.
