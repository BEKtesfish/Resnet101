# ResNet-101 for Pneumonia Detection

This repository contains a modified implementation of ResNet-101 for detecting pneumonia from chest X-ray images.

## Dataset

The dataset consists of images categorized into two classes:
- NORMAL: Images of normal chest X-rays.
- PNEUMONIA: Images indicating pneumonia in chest X-rays.

## Model Architecture

The model architecture is based on ResNet-101 with custom modifications:
- Custom convolutional and identity blocks tailored for pneumonia detection.
- Data augmentation to enhance model robustness.

## Implementation Details

### Data Loading and Preprocessing
- Images are loaded from directories and resized to (64x64) pixels.
- Data augmentation includes random flipping and rotation.

### Training
- Adam optimizer with a base learning rate of 0.00015.
- Early stopping is used based on validation loss to prevent overfitting.

### Evaluation
- Performance metrics on training, validation, and test sets:
  - Accuracy, loss, confusion matrix, and classification report.

## Results

The model achieved the following results on the test set:
- Accuracy: 95.22%
- Loss: 0.1447
- Precision, recall, and F1-score metrics for both classes.

## Usage

To train the model:
1. Ensure TensorFlow and necessary dependencies are installed.
2. Download the dataset and organize it into appropriate directories.
3. Run the training script and monitor the training process.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- This implementation is inspired by the ResNet-101 architecture proposed in the original research papers.
- Thanks to [OpenAI](https://www.openai.com) for providing the foundational knowledge and tools.

