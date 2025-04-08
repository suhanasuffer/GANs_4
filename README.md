# GANs: A Comparative Study

This repository contains a comparative analysis of different types of Generative Adversarial Networks (GANs) implemented on the MedNIST dataset. The primary objective is to evaluate and compare the performance of:
- Least Squares GAN (LS-GAN)
- Wasserstein GAN (WGAN)
- Wasserstein GAN with Gradient Penalty (WGAN-GP)

## Contents

- `ganslab-experiment4-4o.ipynb`: The main experiment notebook with implementation and results
- `README.md`: This file
- Model checkpoints, generated image samples, and evaluation metrics

## Evaluation Metrics

To assess and compare the performance of GANs, the following evaluation methods were used:
- Inception Score (IS)
- Fréchet Inception Distance (FID)
- Visual comparison of generated images

## Tech Stack

- Python
- PyTorch
- TensorBoard (for visualization)
- Matplotlib / Seaborn (for plotting metrics)
- Google Colab or Jupyter Notebook

## Dataset

The experiments are conducted using the **MedNIST** dataset, which includes a variety of medical images from different categories.

## Objective

The goal of this project is to:
- Understand and implement various GAN architectures
- Observe how loss functions affect the training and output quality
- Compare generated outputs using both qualitative and quantitative metrics

## Key Learnings

- GAN training stability varies significantly across architectures
- WGAN-GP generally offers better stability and image quality
- FID provides better insights compared to IS in some medical contexts

## Author
 [Suhani Thakur](https://github.com/suhanasuffer)

## License

This project is open-source and free to use under the MIT License.

