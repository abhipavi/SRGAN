# Photo-Realistic Single Image Super-Resolution using a Generative Adversarial Network

Welcome to the Single Image Super-Resolution (SISR) project repository! This project focuses on enhancing the resolution of low-resolution images to produce high-quality, photo-realistic outputs using various deep learning architectures. Below is a detailed guide to help you understand the project's objectives, methodologies, results, and future directions.

## Introduction

Single Image Super-Resolution (SISR) is a classical problem in computer vision that involves recovering a high-resolution image from a single low-resolution input. This project explores different deep learning architectures to tackle this problem, with a focus on achieving photo-realistic outputs.

## Objective

The primary objective of this project is to compare and evaluate different SISR architectures to determine which one produces the most visually pleasing and accurate results. The project also aims to understand the challenges associated with super-resolution, such as detail loss and image smoothing, particularly at high upscaling factors.

## Methodology

### Data and Tools
- The project utilizes the BSD100 dataset for training and testing.
- TensorFlow and Keras frameworks are employed for implementing the deep learning models.
- Google Colab, an open-source platform, is used for executing Python code, especially suited for machine learning tasks.

### Architectures Explored
1. SRCNN (Super Resolution CNN)
2. ESRCNN (Expanded Super Resolution CNN)
3. DSRCNN (Denoising Auto Encoder Super Resolution CNN)
4. DDSRCNN (Deep Denoising Super Resolution CNN)
5. SRResNet (Residual Network Super Resolution)
6. SRGAN (Super Resolution Generative Adversarial Network)
7. ESRGAN (Enhanced Super Resolution Generative Adversarial Network)

### Training
- All models are trained on the BSD100 dataset for 150 epochs using TensorFlow.
- Training is performed on Google Colab with GPU acceleration.
- Models are evaluated for both 2x and 4x upscaling factors.

## Results

The project evaluates the performance of each architecture based on metrics such as Peak Signal-to-Noise Ratio (PSNR), Mean Squared Error (MSE) loss, and Structural Similarity Index (SSIM). Here are the summarized results for 4x upscaling on the BSD100 dataset:

| Model     | PSNR  | SSIM   |
|-----------|-------|--------|
| SRCNN     | 24.14 | 0.6255 |
| ESRCNN    | 23.86 | 0.5996 |
| DSRCNN    | 24.29 | 0.6206 |
| DDSRCNN   | 24.17 | 0.6315 |
| SRResNet  | 24.21 | 0.6294 |
| SRGAN     | 24.64 | 0.6021 |
| ESRGAN    | 25.24 | 0.7801 |

## Conclusion

While all architectures show similar PSNR values, ESRGAN stands out for its ability to preserve fine texture details, especially at higher upscaling factors. The project emphasizes the importance of achieving photo-realistic outputs rather than solely focusing on pixel accuracy.

## Future Work

Future work will focus on further enhancing the proposed ESRGAN architecture to improve SSIM values. Additionally, exploration of other innovative techniques and datasets may lead to even better super-resolution results.

