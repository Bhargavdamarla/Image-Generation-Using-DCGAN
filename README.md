# 🎨 Image Generation Using DCGAN

This project explores the use of Deep Convolutional Generative Adversarial Networks (DCGANs) to generate realistic images from random noise. The model was trained on three datasets of increasing complexity—MNIST, SVHN, and CelebA—to understand how GANs perform on different types of image data.

---

## 🚀 Project Overview

Generative Adversarial Networks (GANs) consist of two neural networks:

- **Generator** – creates synthetic images from random noise.
- **Discriminator** – learns to distinguish real images from generated images.

Both networks compete against each other during training, enabling the generator to gradually produce more realistic images.

In this project, separate DCGAN models were trained on handwritten digits, street-view house numbers, and celebrity face images.

---

## ✨ Features

- Implemented Deep Convolutional GAN (DCGAN) architecture
- Trained models on MNIST, SVHN, and CelebA datasets
- Designed custom Generator and Discriminator networks
- Used Binary Cross Entropy loss and Adam optimizer
- Generated synthetic images from random noise vectors
- Compared model performance across datasets with different complexities
- Analyzed training behavior using loss curves and visual outputs

---

## 🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- OpenCV

---

## 📂 Datasets

### MNIST
A dataset containing 70,000 grayscale images of handwritten digits (0–9). Each image is 28×28 pixels and provides a simple benchmark for evaluating generative models.

### SVHN (Street View House Numbers)
Contains more than 600,000 real-world digit images collected from Google Street View. The dataset is more challenging due to variations in lighting and background.

### CelebA
A large-scale dataset with over 200,000 celebrity face images. The high diversity and image complexity make it significantly harder for the model to generate realistic outputs.

---

## 🧠 Model Architecture

The DCGAN model consists of two components:

### Generator
The generator takes random noise as input and produces synthetic images. It uses transposed convolution layers along with batch normalization and LeakyReLU activations.

### Discriminator
The discriminator acts as a binary classifier and determines whether an image is real or generated. It learns to distinguish fake samples from actual images during training.

---

## ⚙️ Training Configuration

| Parameter | Value |
|------------|--------|
| Optimizer | Adam |
| Learning Rate | 0.0002 |
| Beta1 | 0.5 |
| Loss Function | Binary Cross Entropy |
| Framework | TensorFlow |

---

## 📈 Results

### MNIST
The model was able to generate clear and recognizable handwritten digits. Since the dataset is relatively simple, training converged quickly and produced high-quality outputs.

### SVHN
Generating house numbers was more challenging because of color variations and complex backgrounds. The image quality improved steadily with training, although minor artifacts remained.

### CelebA
The model successfully learned facial structures and generated human-like faces. While some images contained blurring, the generated samples captured important facial features and showed significant improvement over time.

---

## 📊 Evaluation

Model performance was evaluated through:

- Visual inspection of generated samples
- Generator and discriminator loss curves
- Training stability analysis
- Comparison of outputs across different datasets

---

## 📁 Project Structure

```text
Image-Generation-Using-DCGAN
│
├── notebooks/
├── models/
├── outputs/
├── train.py
├── generator.py
├── discriminator.py
├── requirements.txt
└── README.md
```

---

## ⚡ Getting Started

Clone the repository:

```bash
git clone https://github.com/Bhargavdamarla/Image-Generation-Using-DCGAN.git
```

Move to the project directory:

```bash
cd Image-Generation-Using-DCGAN
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

Run the training script:

```bash
python train.py
```

---

## 🔍 Applications

- Synthetic image generation
- Data augmentation
- Generative AI research
- Computer vision applications
- Unsupervised representation learning

---

## 🚀 Future Work

- Explore Wasserstein GAN (WGAN)
- Experiment with StyleGAN architectures
- Improve image quality and resolution
- Use metrics such as FID score for evaluation
- Enhance training stability

---

## 📚 References

- Ian Goodfellow et al., *Generative Adversarial Networks* (2014)
- TensorFlow Documentation
- MNIST Dataset
- SVHN Dataset
- CelebA Dataset

---

## 👨‍💻 Author

**Sai Bhargav Damarla**

📧 saibhargavdamarla@gmail.com  
🔗 LinkedIn: https://linkedin.com/in/saibhargavdamarla  
💻 GitHub: https://github.com/Bhargavdamarla

