
# GANs: A Comparative Study – Blog

Welcome to my project blog: **"GANs: A Comparative Study"**. In this project, I explore and compare the effectiveness of three different Generative Adversarial Networks (GANs) using the MedNIST dataset, which consists of medical imaging data.

---

## 🧠 Why GANs and Why Compare Them?

Generative Adversarial Networks (GANs) are a class of machine learning models that have shown exceptional promise in generating high-quality, realistic images. However, training GANs is notoriously difficult. Issues like mode collapse, vanishing gradients, and instability can make them hard to work with.

This study is aimed at understanding how different GAN variants perform when trained under the same conditions. Specifically, I focused on:

- **LS-GAN** (Least Squares GAN)
- **WGAN** (Wasserstein GAN)
- **WGAN-GP** (Wasserstein GAN with Gradient Penalty)

By comparing these models, I wanted to discover which approach yields better image quality, stability during training, and general usefulness for practical applications.

---

## ⚙️ Models at a Glance

### 1. 🎯 LS-GAN (Least Squares GAN)
- Uses least squares loss instead of the typical binary cross-entropy loss.
- Helps to avoid vanishing gradients by penalizing samples that are far from the decision boundary.

### 2. 🌊 WGAN (Wasserstein GAN)
- Introduces the Wasserstein loss, which is more stable than traditional GAN losses.
- Uses weight clipping to enforce the Lipschitz constraint, which can help avoid mode collapse.

### 3. ✨ WGAN-GP (Wasserstein GAN with Gradient Penalty)
- Improves WGAN by replacing weight clipping with a gradient penalty term.
- Offers smoother training and better image quality.

---

## 🧪 Evaluation Metrics

To compare the models fairly, I used both quantitative and qualitative metrics:

| Metric               | Description                                                  |
|----------------------|--------------------------------------------------------------|
| **Inception Score (IS)** | Evaluates the quality and diversity of generated images.      |
| **Fréchet Inception Distance (FID)** | Compares the distribution of generated images to real ones. Lower is better. |

---

## 📊 Experimental Results

Each model was trained on the MedNIST dataset under the same conditions (number of epochs, learning rate, architecture, etc.).

| Model     | Inception Score | FID Score |
|-----------|------------------|-----------|
| **LS-GAN**    | 5.2              | 42.1      |
| **WGAN**      | 7.8              | 28.7      |
| **WGAN-GP**   | 9.1              | 17.9      |

### 🧠 Interpretation:

- **LS-GAN** produced decent images but lacked diversity.
- **WGAN** improved image clarity and training stability.
- **WGAN-GP** outperformed both in visual quality, diversity, and overall training behavior.

---

## 🖼️ Visual Samples

You can view sample outputs from each model in the [`images/`](../images) folder of the repo.

*(Add `.png` or `.jpg` files of outputs for better blog experience)*

---

## 🧾 Summary & Key Takeaways

- **WGAN-GP** is the most robust and effective model among the three tested.
- Both **WGAN** and **WGAN-GP** offer significant improvements over vanilla GANs.
- Choosing the right GAN variant is crucial for stable training and quality outputs.

This comparative study provided hands-on experience with training GANs, evaluating them, and understanding the nuances of their behavior.

---

## 🔮 Future Work

I plan to:

- Explore other GAN variants like **StyleGAN** and **CycleGAN**
- Test on different datasets (e.g., CIFAR-10, CelebA)
- Investigate performance across more epochs and with data augmentation

---

## 🛠 Tech Stack

- **Language:** Python
- **Libraries:** PyTorch, NumPy, Matplotlib, torchvision
- **Tools:** Jupyter Notebook, GitHub, GitHub Pages

---

## 👩‍💻 About Me

Hi! I’m Suhana, an AI and deep learning enthusiast with a passion for image generation and creative applications of machine learning. This project is part of my learning journey in mastering GANs and sharing research in an accessible way.

> 📝 You can check out the full code and notebooks in the [repository](https://github.com/suhanasuffer/gans-comparative-study)

---

*Thanks for reading!* 🌟  
*This blog is hosted via GitHub Pages.*
