# Attention-Augmented-Convolutional-Networks
This is a pytorch implementation of the paper [Attention Augmented Convolutional Networks](https://arxiv.org/abs/1904.09925 "Attention Augmented Convolutional Networks")

## Method
The paper implements the attention mechanism into different ResNet architectures. Convolutional and attentional feature maps are concatenated in a choosen ratio.

![aacn_image](https://user-images.githubusercontent.com/19909320/119885192-cd15e900-bf31-11eb-985b-be4e09ac9a4c.png)

*  ![v](https://user-images.githubusercontent.com/19909320/119885127-b40d3800-bf31-11eb-8165-1b12a739179f.png) 
is the ratio of attentional channels to number of original output filters

* ![k](https://user-images.githubusercontent.com/19909320/119885316-f9316a00-bf31-11eb-96e4-97134fc0dfb1.png) 
is the ratio of key depth to number of original output filters

![AACN](https://user-images.githubusercontent.com/19909320/137499701-4cace468-ffa5-4b2e-b15f-14d2ddee4fbf.png)

## Disclaimer

This design is inspired by the work of [MartinGer](https://github.com/MartinGer). Full credit to him for the foundational ideas.

## Implementation Details

Advanced architectures such as **ResNet-50**, **Wide-ResNet**, and experiments on large-scale datasets like **CIFAR-100** and **ImageNet** are available in:

- [`AACN_Layer`](#AACN_Layer)  
- [`AACN_Model`](#AACN_Model)

For a more lightweight and educational example, I implemented an **Attention Augmented ResNet-18** tailored for the **CIFAR-10** dataset. It stays true to the core ideas of the original paper and can be found in:

- [`attention-augmented-cnns.ipynb`](#attention-augmented-cnnsipynb)

For a comparative analysis between **AA-ResNet** and the standard **ResNet**, see:

- [`Standard_ResNet.ipynb`](#standard_resnetipynb)



