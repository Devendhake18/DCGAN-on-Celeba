# DCGAN for CelebA Face Generation

This repository contains an implementation of a Deep Convolutional Generative Adversarial Network (DCGAN) for generating face images using the CelebA dataset.

## Dataset Preprocessing

1. **Download the CelebA dataset**: Ensure you have the `img_align_celeba` dataset.
2. **Set the dataset path**: Modify the `dataroot` variable in the script to point to the dataset folder.
3. **Transformations applied**:
   - Resize images to `64x64`.
   - Center crop images.
   - Convert images to tensors.
   - Normalize images to range `[-1, 1]`.

     ![image](https://github.com/user-attachments/assets/708baaf4-c4bc-49d9-9a67-3e339b11ddba)


## Training the Model

### Prerequisites

- Python 3.x
- PyTorch
- TorchVision
- Matplotlib
- NumPy

### Steps to Train

1. Clone the repository:
   ```sh
   git clone <repository-url>
   cd dcgan-celeba
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the training script:
   ```sh
   python train.py
   ```

## Testing the Model

1. Once trained, generate fake images using the saved model.
2. Modify the script to load the trained generator and generate samples.

## Expected Outputs

- The model generates 64x64 images of human faces.
- Loss curves for generator and discriminator.
- Comparison between real and generated images.

  ![image](https://github.com/user-attachments/assets/e32c112c-66ca-4694-a775-006eeb4c3fca)


## Repository Structure

```
|-- dataset/            # Folder containing CelebA images
|-- train.py            # Main training script
|-- models.py           # Generator and Discriminator models
|-- utils.py            # Utility functions
|-- README.md           # Documentation
```

## Contact

For any issues, feel free to open an issue on GitHub.

