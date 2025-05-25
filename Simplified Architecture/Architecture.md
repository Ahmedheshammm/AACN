# Attention Augmented Convolutional Networks on CIFAR-10

This repository compares the performance of a standard ResNet-18 and an Attention Augmented ResNet (AA-ResNet) based on the architecture proposed in [Bello et al., 2019](https://arxiv.org/abs/1904.09925).

## 📁 Files

- `standard-resnet.ipynb`: Implementation and training of standard ResNet-18 on CIFAR-10.
- `attention-augmented-cnns.ipynb`: Modified ResNet-18 with self-attention modules in selected convolution layers.

## 🧠 Model Architecture

- **Standard ResNet-18**: Baseline CNN without attention.
- **AA-ResNet-18**: Integrates multi-head self-attention into selected convolution layers.

## 📊 Dataset

- **CIFAR-10**: 60,000 32×32 color images in 10 classes.
- Train/Test split: 50,000 / 10,000.

## 🏋️ Training Details

- Learning rate: `0.1`
- Batch size: `128`
- Number of epochs: `160-200`
- Loss: CrossEntropyLoss with label smoothing (ε = 0.1)
- Optimizer: SGD + Momentum
- Scheduler: MultiStepLR
- Epochs: 160 (ResNet), 200 (AA-ResNet)
- Evaluation: Accuracy, Per-Class Accuracy, Visualization

