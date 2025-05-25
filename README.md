# Attention-Augmented Convolutional Networks

---

This repository contains a PyTorch implementation of the paper "[Attention Augmented Convolutional Networks](https://arxiv.org/abs/1904.09925)".

## Overview

This project explores the integration of attention mechanisms into various ResNet architectures. The core idea involves concatenating convolutional and attentional feature maps in a chosen ratio, as depicted below:

![Attention-Augmented Convolutional Block](https://user-images.githubusercontent.com/19909320/119885192-cd15e900-bf31-11eb-985b-be4e09ac9a4c.png)

* $v$: Represents the ratio of attentional channels to the number of original output filters.
* $k$: Denotes the ratio of key depth to the number of original output filters.

Below is a high-level representation of the Attention Augmented Convolutional Network:

![Attention Augmented Convolutional Network](https://user-images.githubusercontent.com/19909320/137499701-4cace468-ffa5-4b2e-b15f-14d2ddee4fbf.png)

---

## Disclaimer

This design is inspired by the work of [MartinGer](https://github.com/MartinGer). Full credit to him for the foundational ideas.

## Repository Structure

This repository is organized to provide both detailed and simplified architectural examples:

* **`Fully detailed Architecture/`**: Contains advanced implementations, including **ResNet-50**, **Wide-ResNet**, and experiments on large-scale datasets like **CIFAR-100** and **ImageNet**. You'll find:
    * [`AACN_Layer`](Fully%20detailed%20Architecture/AACN_Layer)
    * [`AACN_Model`](Fully%20detailed%20Architecture/AACN_Model)

* **`Simplified Architecture/`**: Offers a more lightweight and educational example. This section features an **Attention Augmented ResNet-18** specifically tailored for the **CIFAR-10** dataset, staying true to the core ideas of the original paper.
    * [`attention-augmented-cnns.ipynb`](Simplified%20Architecture/attention-augmented-cnns.ipynb)

* **`Important README/`**: For a comparative analysis between **AA-ResNet** and the standard **ResNet**, see:
    * [`Standard_ResNet.ipynb`](Important%20README/Standard_ResNet.ipynb)

---





