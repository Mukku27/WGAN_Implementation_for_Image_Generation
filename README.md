## WGAN Implementation for Image Generation

This repository implements a Wasserstein Generative Adversarial Network (WGAN) for image generation, inspired by the research paper "Improved Training of Wasserstein GANs" ([https://arxiv.org/abs/1704.00028](https://arxiv.org/abs/1704.00028)).

**Key Components:**

* **model_wgan.py:** Defines the Discriminator and Generator architectures with convolutional layers and leaky ReLU activations.
* **utils.py:** Contains the `gradient_penalty` function for enforcing gradient clipping in WGANs.
* **train_WGAN.ipynb:** Implements the training loop with logging and visualization.

**Installation:**

1. Clone or download the repository.
2. Install required dependencies: `torch`, `torchvision`, and any other necessary libraries.

**Usage:**

1. Ensure `celeb_dataset` contains your training images in an appropriate format (e.g., subfolders for different classes).
2. Run `train_WGAN.ipynb` using a Jupyter Notebook environment or a Python script execution tool.
3. Adjust hyperparameters in `train_WGAN.ipynb` (e.g., `LEARNING_RATE`, `Batch_size`, etc.) as needed.
4. Visualize TensorBoard logs (usually located at `http://localhost:6006`) to track training progress and generated images.

**Additional Notes:**

* This implementation is a foundation for WGAN. Further improvement might involve spectral normalization, hyperparameter tuning, or advanced architectures.
* Consider providing scripts for data preprocessing and evaluation metrics.
* Include clear comments and docstrings in code for better readability.

**Resources:**

* **Improved Training of Wasserstein GANs:** [https://arxiv.org/abs/1704.00028](https://arxiv.org/abs/1704.00028)
* **WGAN Blog:** [https://www.alexirpan.com/2017/02/22/wasserstein-gan.html](https://www.alexirpan.com/2017/02/22/wasserstein-gan.html)
