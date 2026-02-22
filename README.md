# CIFAR-10 Image Classification

Comparing three deep learning models (SimpleNN, AlexNet, TinyVGG) on CIFAR-10
using PyTorch. Models are evaluated on accuracy, F1 score, training time, and
parameters. Trained on Google Colab with GPU acceleration.

---

## What is this project?

This project teaches computers to recognise images.
We train three different AI models to look at a photo and answer:
**"Is this a cat, dog, car, plane...?"**

We then compare which model is the smartest, fastest, and most efficient.

---

## What is CIFAR-10?

CIFAR-10 is a collection of **60,000 small images** split into 10 categories:

✈️ Airplane | 🚗 Car | 🐦 Bird | 🐱 Cat | 🦌 Deer
🐶 Dog | 🐸 Frog | 🐴 Horse | 🚢 Ship | 🚛 Truck

- 50,000 images used for training
- 10,000 images used for testing

---

## The Three Models We Compare

### 1. SimpleNN (Basic Neural Network)
- The simplest model — just a few layers of connected neurons
- Like a student who memorises answers without understanding the topic
- Used as our starting point to see how much better we can do

### 2. AlexNet
- A famous model that won a major AI competition in 2012
- Much smarter — it looks at groups of pixels to understand shapes and patterns
- We adapted it to work with CIFAR-10's small images

### 3. TinyVGG
- A smaller, simpler version of a powerful model called VGG
- Fast to train and works really well on small images like CIFAR-10
- Uses small 3×3 filters to detect patterns step by step

---

## How We Trained the Models

| Setting | Value | Plain English |
|---|---|---|
| Optimizer | Adam | The method used to improve the model after each guess |
| Loss Function | CrossEntropyLoss | How we measure how wrong the model is |
| Batch Size | 128 | How many images the model looks at at once |
| Epochs | 30 | How many times the model sees the full dataset |
| Hardware | Google Colab T4 GPU | Free online GPU used to speed up training |

---

## How We Measured Performance

- **Accuracy** — out of 100 images, how many did it get right?
- **Precision** — when it says "cat", how often is it actually a cat?
- **Recall** — out of all real cats, how many did it find?
- **F1 Score** — a combined score of precision and recall
- **Training Time** — how long did it take to learn?
- **Parameters** — how complex is the model?

---

## What We Found

- TinyVGG performed the best overall
- SimpleNN was the weakest — it cannot understand image structure
- AlexNet proved that its 2012 innovations still work well today
- Cat vs Dog and Car vs Truck were the hardest to get right

---

## How to Run This Project

1. Open the notebook in **Google Colab**
2. Enable free GPU: **Runtime → Change runtime type → T4 GPU**
3. Run everything: **Runtime → Run all**
4. Watch the models train and compare results at the end

---

## Files
```
├── CNN(AlexNet).ipynb  # The main notebook
└── README.md                                     # This file
```

---

## 📚 References
- AlexNet Paper — Krizhevsky, Sutskever & Hinton (2012)
- [PyTorch Documentation](https://pytorch.org)
- [CIFAR-10 Dataset](https://www.cs.toronto.edu/~kriz/cifar.html)
