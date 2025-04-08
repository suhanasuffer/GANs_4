
# GANs: A Comparative Study

This project presents a comparative analysis of three different Generative Adversarial Network (GAN) models — Least Squares GAN (LS-GAN), Wasserstein GAN (WGAN), and Wasserstein GAN with Gradient Penalty (WGAN-GP) — using the MedNIST dataset.

## 📌 Project Goals

- Compare the performance of LS-GAN, WGAN, and WGAN-GP.
- Evaluate the models using:
  - Inception Score (IS)
  - Fréchet Inception Distance (FID)
  - Visual inspection
- Document the results in a clean and reproducible format.

## 🧠 Models Implemented

- **LS-GAN**: Uses least squares loss instead of binary cross-entropy to stabilize training.
- **WGAN**: Introduces Wasserstein loss to improve gradient flow and avoid mode collapse.
- **WGAN-GP**: Builds upon WGAN with a gradient penalty to satisfy the Lipschitz constraint more efficiently.

## 📊 Evaluation Metrics

- **Inception Score (IS)**: Measures image quality and diversity.
- **Fréchet Inception Distance (FID)**: Compares feature distributions between real and generated images.
- **Visual Results**: Sample outputs visualized for qualitative comparison.

## 📷 Sample Results

| Model     | Inception Score | FID Score |
|-----------|------------------|-----------|
| LS-GAN    | 5.2              | 42.1      |
| WGAN      | 7.8              | 28.7      |
| WGAN-GP   | 9.1              | 17.9      |

> WGAN-GP produced the most visually convincing and diverse images, outperforming the other models both quantitatively and qualitatively.

## 🌐 GitHub Pages Blog

View the detailed blog post [here](https://suhanasuffer.github.io/gans-comparative-study)

## 🛠 Technologies Used

- Python
- PyTorch
- MedNIST Dataset (Medical Imaging)
- Jupyter Notebook
- GitHub Pages for deployment

