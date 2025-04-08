
# GANs: A Comparative Study – Blog

Welcome to the blog version of my project **"GANs: A Comparative Study"**. This project explores and compares the performance of three different types of GANs (Generative Adversarial Networks) on the MedNIST medical imaging dataset.

---

## 🧠 Why GANs?

GANs have revolutionized image generation, but their training can be unstable. This motivated the need to explore and compare different GAN variants under the same conditions.

---

## ⚙️ Models Compared

### 1. Least Squares GAN (LS-GAN)
- Replaces binary cross-entropy with least squares loss.
- Aims to provide smoother gradients.

### 2. Wasserstein GAN (WGAN)
- Uses Wasserstein distance for better convergence.
- Enforces Lipschitz constraint via weight clipping.

### 3. Wasserstein GAN with Gradient Penalty (WGAN-GP)
- Improves upon WGAN by adding a gradient penalty.
- Avoids weight clipping and stabilizes training further.

---

## 🧪 Evaluation Metrics

| Metric               | Description                                                  |
|----------------------|--------------------------------------------------------------|
| Inception Score (IS) | Measures image quality and diversity                         |
| FID Score            | Measures similarity between generated and real image features|

---

## 📈 Results Summary

| Model     | Inception Score | FID Score |
|-----------|------------------|-----------|
| LS-GAN    | 5.2              | 42.1      |
| WGAN      | 7.8              | 28.7      |
| WGAN-GP   | 9.1              | 17.9      |

WGAN-GP outperformed the others in terms of both quality and diversity of images.

---

## 🖼️ Visual Samples

> *(Add generated image samples in the `docs/images` folder and embed them here)*

---

## 🚀 Conclusion

This comparative study demonstrates that WGAN-GP provides the most stable training and best output quality among the tested models. More advanced GAN architectures can be explored in the future to further enhance results on complex datasets.

---

*Project by [Suhana](https://github.com/suhanasuffer)*  
*Hosted via GitHub Pages*
