# Deep Learning project 

# 🧥 Fashion Image Generator using GAN & Diffusion Models

This project is a **Fashion Image Generator** built using a hybrid of **Generative Adversarial Networks (GANs)** and **Diffusion Models**. It generates realistic fashion item images (such as shirts, shoes, and bags) trained on the **FashionMNIST dataset**.

---

## 🚀 Project Overview

This project combines the power of **GANs** (for adversarial image generation) with **Diffusion Models** (for refining and denoising generated samples).  
The goal is to synthesize **high-quality fashion images** that resemble real dataset samples while maintaining diversity and clarity.

### ✨ Features
- Trains a **hybrid GAN + Diffusion model** to generate fashion images.
- Uses **FashionMNIST**, a lightweight dataset of 70,000 grayscale fashion images.
- Generates **new and unique fashion items**.
- Implements **denoising diffusion steps** for image refinement.
- Includes visualizations of **training progress**, **loss curves**, and **generated outputs**.

---

## 🧠 Model Architecture

### 1. **Generator (GAN Component)**
- Takes random noise (`z`) as input.
- Produces low-resolution fashion-like images.
- Uses convolutional transpose layers with batch normalization.

### 2. **Discriminator**
- Classifies images as *real* or *fake*.
- Trains adversarially against the generator.

### 3. **Diffusion Refinement**
- Adds a **diffusion-based noise reduction** step.
- Gradually refines GAN-generated samples to enhance quality and reduce artifacts.

---

## 🧰 Tech Stack

| Component | Technology |
|------------|-------------|
| Language | Python |
| Frameworks | TensorFlow / PyTorch (depending on notebook implementation) |
| Dataset | [FashionMNIST](https://github.com/zalandoresearch/fashion-mnist) |
| Visualization | Matplotlib, Seaborn |
| Training | GAN + Diffusion model pipeline |

---

## 📂 Dataset

**FashionMNIST** contains:
- 60,000 training images
- 10,000 testing images
- 10 fashion categories:
  - T-shirt/top
  - Trouser
  - Pullover
  - Dress
  - Coat
  - Sandal
  - Shirt
  - Sneaker
  - Bag
  - Ankle boot

Each image is **28×28 pixels**, grayscale.

---
