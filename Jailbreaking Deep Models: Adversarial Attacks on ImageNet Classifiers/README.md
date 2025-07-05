# Jailbreaking Deep Models: Adversarial Attacks on ImageNet Classifiers

This project investigates the vulnerability of deep neural networks to adversarial attacks using the ImageNet dataset and pretrained models like ResNet-34 and DenseNet-121.

## Objective

- Simulate pixel-wise and patch-based adversarial attacks
- Evaluate model degradation under attacks
- Analyze transferability across models

## Methods Used

| Attack Type     | Top-1 Accuracy | Top-5 Accuracy |
|-----------------|----------------|----------------|
| Original        | 74.80%         | 93.60%         |
| FGSM (ε=0.02)   | 06.20%         | 35.40%         |
| PGD (ε=0.02)    | 00.00%         | 07.80%         |
| Patch Attack    | 30.60%         | 50.80%         |

### Insights

- FGSM and PGD cause drastic drops in classification performance even with minimal perturbation.
- Patch attacks generalize better across models and cause sharp accuracy declines.
- Attacks designed on ResNet-34 retain high transferability when applied to DenseNet-121.

## Visualizations

Each attack includes:
- Original vs Adversarial image
- Perturbation heatmap
- Output label comparison

## Tech Stack

- PyTorch
- Torchvision
- NumPy, Matplotlib, TQDM
- Pretrained models from ImageNet

## How to Run

1. Open the notebook: `dl-project.ipynb`
2. Ensure the ImageNet dataset and pretrained models are accessible.
3. Run the notebook blocks for FGSM, PGD, and Patch attacks.
4. Outputs (visuals and metrics) will be generated locally.
