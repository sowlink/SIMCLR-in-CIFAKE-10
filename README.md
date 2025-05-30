# Project Purpose
This is the part of university project I have done in Deep Learning course.
The dataset is used by CIFAR-10 (Krizhevsky & Hinton, 2009)& AI-generated synthetic images from Stable Diffusion (Bird & Lotfi, 2024)
The images from these datasets are applied Simple Framework for Contrastive Learning (SimCLR), and this is the method of learning by capturing diverse visual patterns, enhancing feature generalizability without relying on labels. You could reference from the code.
The unseen part is from my groupmate. He has proposal and done with a Wasserstein Generative Adversarial Network with Gradient Penalty (wGAN-GP) to enhance the quality (MIGHT FROM LOW TO HIGH) and semantic consistency of generated images. [this part would not share, as there is no permission]

## Hardware
- Training was performed on the university’s NVIDIA GPUs (accessed via `nvidia-smi`).
- Configuration: 8 GPUs with a total of 48 GB VRAM

## Features
- **Loss Function**: Uses Normalized Temperature-scaled Cross Entropy Loss (NT-Xent) to optimize contrastive learning.
- **Training Setup**:
  - 128-dimensional feature extraction.
  - Learning rate: 0.01.
  - Number of epochs: 20.
- **Downstream Tasks**:
  - Logistic regression and fine-tuning, both with a learning rate of 0.001.

## The following improvement
- Try the different GAN models
- Use a more clear datasets (32x32 is too small)
- Use a higher quality GPU
[YOU COULD COMMENT A BETTER WAY TO RUN THIS CODE AND USE OTHER EFFECTIVE METHOD]

## References
Krizhevsky, A., & Hinton, G. (2009). Learning multiple layers of features from tiny images. 
University of Toronto. 

Pandey, M., Singh, S., Malik, A., & Kumar, R. (2024). Detecting low-resolution deepfakes: An 
exploration of machine learning techniques. Multimedia Tools and Applications, 83(25), 
66283–66298. https://doi.org/10.1007/s11042-024-18235-7 
