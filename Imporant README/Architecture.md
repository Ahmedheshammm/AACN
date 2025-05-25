## Architecture

The implementation includes:

- A smaller-scale version of **Attention Augmented ResNet-18**, adapted for the **CIFAR-10** dataset.
- A baseline **standard ResNet-18** model (without attention) for direct comparison.
- Attention modules are integrated into the residual blocks following the original paper's design, with scaled-down parameters to fit the CIFAR-10 task.

## Model Variants

- `AA_ResNet18`: ResNet-18 with attention-augmented convolution layers.
- `Standard_ResNet18`: Standard ResNet-18 without attention.

## Files

- `attention-augmented-cnns.ipynb`: Main notebook implementing AA-ResNet18.
- `Standard_ResNet.ipynb`: Notebook implementing standard ResNet18 for comparison.

## Design Choices

- Chosen dataset: **CIFAR-10**
- Model depth: **ResNet-18**
- Input image size: `32x32`
- Attention settings:
  - Number of heads: `8`
  - Relative positional encodings: `enabled/disabled`
  - Attention width ratio (k): `...`

## Training Details

- Optimizer: `SGD`
- Learning rate: `0.1`
- Batch size: `128`
- Number of epochs: `160-200`
- Scheduler (if any): `...`
- Loss function: `CrossEntropyLoss`
