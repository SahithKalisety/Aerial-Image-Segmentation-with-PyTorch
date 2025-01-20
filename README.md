# Aerial-Image-Segmentation-with-PyTorch

This project demonstrates aerial image segmentation using PyTorch, focusing on classifying pixels in aerial images to identify specific regions such as roads. The implementation leverages pre-trained models from the `segmentation-models-pytorch` library, combined with data augmentation and preprocessing techniques for improved performance.

## Features
- **State-of-the-Art Models**: Utilizes pre-trained models from `segmentation-models-pytorch` for efficient and accurate segmentation.
- **Data Augmentation**: Implements augmentation strategies using `albumentations` to improve model generalization.
- **Modular Design**: Easy-to-customize scripts for training, evaluation, and preprocessing.

## Dataset
The dataset is sourced from the [Road_seg_dataset](https://github.com/parth1620/Road_seg_dataset). It contains labeled aerial images suitable for semantic segmentation tasks. Clone this dataset using:
```bash
git clone https://github.com/parth1620/Road_seg_dataset.git
```
Ensure the dataset structure matches the expected format in the training scripts.

## Installation

### Prerequisites
- Python 3.8 or higher
- CUDA-enabled GPU (optional but recommended for faster training)

### Steps
1. Clone this repository and navigate to the project directory:
   ```bash
   git clone <repository_url>
   cd <repository_name>
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Clone the dataset repository:
   ```bash
   git clone https://github.com/parth1620/Road_seg_dataset.git
   ```

4. Add the dataset path to your Python path:
   ```python
   import sys
   sys.path.append('/path/to/Road_seg_dataset')
   ```

## Requirements
See `requirements.txt` for the list of dependencies. Key libraries include:
- PyTorch
- segmentation-models-pytorch
- albumentations
- OpenCV

## Hardware Recommendations
- NVIDIA GPU with CUDA support for faster training and inference.
- At least 16GB RAM for processing high-resolution images.

## Acknowledgments
- [segmentation-models-pytorch](https://github.com/qubvel/segmentation_models.pytorch) for pre-trained models.
- [Albumentations](https://github.com/albumentations-team/albumentations) for data augmentation.
- [Road_seg_dataset](https://github.com/parth1620/Road_seg_dataset) for the dataset.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.
