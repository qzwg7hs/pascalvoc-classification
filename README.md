# Pascal VOC 2012 – Single-Label Image Classification

Final project for the **Yessenov Data Lab 2025**: transforming a multi-label object detection dataset into a single-label image classification task using deep learning.

## Dataset

- Source: [Pascal VOC 2012](https://pytorch.org/vision/stable/generated/torchvision.datasets.VOCDetection.html)
- Originally multi-label (objects + bounding boxes)
- Preprocessed by cropping individual objects to generate single-label classification data

## Models Used

- Custom CNN (built from scratch)
- Pretrained models (fine-tuned with head-only and full modes):
  - ResNet50
  - EfficientNet-B0
  - MobileNetV3
  - ShuffleNetV2
  - ConvNeXt-Tiny

## Techniques

- Dataset balancing (e.g., pruning overrepresented "person" class)
- Image segmentation
- Hyperparameter search: learning rate, optimizer (Adam, SGD), batch size
- Evaluation: accuracy, F1-score, confusion matrix

## Best Results

- **MobileNetV3 (Adam, head-only)**: **82.78% test accuracy**

## Files

- `notebooks/`: Jupyter notebooks for training, fine-tuning, and EDA
- `Model Report.pdf`: Full project report
- `requirements.txt`: Python dependencies

## Team: Tassay aka MARS

- Makhmud, Aruay, Ruana, Sanzhar

