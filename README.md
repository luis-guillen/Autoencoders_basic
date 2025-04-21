# Autoencoders Basic - Upscale MNIST

This repository is dedicated to showcasing the use of autoencoders for enhancing the resolution of images, specifically targeting the MNIST dataset. The project demonstrates how to train an autoencoder to reconstruct high-resolution images from their low-resolution counterparts.

## Overview

The **Upscale MNIST** project aims to reduce the dimensions of MNIST images and then reconstruct their original resolution using an autoencoder. This approach can be applied to various real-world applications, such as image enhancement, compression, and preprocessing for machine learning tasks.

Key highlights:
- Use of the MNIST dataset for training and evaluation.
- Implementation of an autoencoder architecture with a convolutional encoder and decoder.
- Side-by-side comparison of original, low-resolution, and reconstructed images.

## Features

- **Data Preparation**:
  - MNIST images are resized to half their original dimensions as input to the autoencoder.
  - The autoencoder learns to reconstruct the original resolution.

- **Autoencoder Architecture**:
  - Encoder: Compresses the input image into a latent-space representation.
  - Decoder: Reconstructs the high-resolution image from the latent-space representation.

- **Training and Evaluation**:
  - Loss function: Mean Squared Error (MSE).
  - Optimizer: Adam optimizer for quick convergence.
  - Visualizations of input, downsampled, and reconstructed images to track performance.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/luis-guillen/Autoencoders_basic.git
   cd Autoencoders_basic
   ```

2. Install the required dependencies:
   ```bash
   pip install torch torchvision matplotlib
   ```

## Usage

### Running the Notebook

1. Open the `UpscaleMnist.ipynb` notebook in Jupyter Notebook or JupyterLab.
2. Follow the steps in the notebook to:
   - Prepare the MNIST dataset.
   - Train the autoencoder on the resized images.
   - Evaluate the reconstruction quality on the validation dataset.
3. Visualize the results to compare the original, downsampled, and reconstructed images.

### Example Results

After training the autoencoder:
- The loss decreases gradually over epochs, indicating improved reconstruction quality.
- Reconstructed images effectively restore details from the downsampled inputs.

## Directory Structure

```
Autoencoders_basic/
├── UpscaleMnist.ipynb  # Main notebook for the project
├── README.md           # Project documentation
```

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request if you have ideas for improving this project.

## License

This project is licensed under the Apache 2.0 License. See the [LICENSE](./LICENSE) file for more details.
