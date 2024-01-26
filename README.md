# Handwritten Digit Denoising Autoencoder
## Dimensionality Reduction through Feature Extraction
### Introduction
This project implements a denoising autoencoder using the Keras library and manually using NumPy to reduce the dimensionality of handwritten digits from the MNIST database. The autoencoder takes noisy images as input, reduces their dimensionality, extracts important features, and then reconstructs them to produce denoised images.

### Dataset
The MNIST dataset contains grayscale images of handwritten digits (0-9), each of size 28x28 pixels.

### Overview
- **Pre-trained Encoder:** Implemented using Keras, it maps noisy images to a lower-dimensional representation (784 -> 100).
- **Custom Decoder Layer:** Implemented through linear algebra using NumPy, it reconstructs the images from the lower-dimensional representation through weights found by gradient descent optimization.
- **Comparison with Keras Decoder:** The custom decoder layer is compared to the decoder layers provided by Keras using different optimizers, specifically "SGD" and "Adam".

### Technologies
- Python 3.10
- NumPy
- scikit-learn
- Matplotlib
- Keras


### Results
The custom decoder layer outperforms the Keras decoder with the "SGD" optimizer, however, performs slightly worse than the Keras decoder with the "Adam" optimizer.

*Manual implementation decoded image reconstruction.* 

![image](https://github.com/JSB-0/Denoise_Auto_6348/assets/18308535/e5c09227-cbe2-4626-9390-0403098f7dae)




*Keras "SGD" implementation image reconstruction.* 

![image](https://github.com/JSB-0/Denoise_Auto_6348/assets/18308535/5e960545-3b99-41a9-81aa-37b5498dcb0f)




*Keras "Adam" implementation image reconstruction.*

![image](https://github.com/JSB-0/Denoise_Auto_6348/assets/18308535/21ca63a2-82da-4601-b335-5352e8a27b2e)




