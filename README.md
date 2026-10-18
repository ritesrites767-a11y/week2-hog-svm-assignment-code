# Week 2 Assignment: HOG Features and Image Classification

## Project Overview
This project implements Histogram of Oriented Gradients (HOG) feature extraction and compares two classical machine learning classifiers for image recognition: Linear Support Vector Machine (Linear SVM) and k-Nearest Neighbors (k-NN).

## Dataset
The dataset contains three classes:
- Cats: 25 images
- Dogs: 25 images
- Birds: 25 images

Total: 75 images.

The images were selected from the CIFAR-10 dataset using its test images. Each class contains at least 25 images.

## HOG Feature Extraction
Two HOG configurations are compared:

**Setting A**
- Orientations: 9
- Pixels per cell: 8 × 8
- Cells per block: 2 × 2

**Setting B**
- Orientations: 9
- Pixels per cell: 16 × 16
- Cells per block: 2 × 2

The extracted feature arrays are saved in the `features/` folder. Original images and HOG visualizations are saved in the `visualizations/` folder.

## Classifier Comparison
The classifiers are evaluated using an 80/20 train-test split.

| Classifier | Accuracy |
|---|---:|
| Linear SVM | 66.67% |
| k-NN (k=5) | 26.67% |

Linear SVM performed better on this test split. Results may vary with different data splits and parameters.

## Project Files
- `extract_features.py` — extracts HOG features.
- `compare_classifiers.py` — trains and evaluates classifiers.
- `features/` — saved HOG feature arrays.
- `visualizations/` — HOG comparison images.
- `analysis.md` — analysis and answers to assignment questions.
- `classifier_results.txt` — classification results.
- `dataset/` — image dataset.

## How to Run
Run the Python scripts in a Python environment with the required libraries installed, including NumPy, Matplotlib, scikit-image, and scikit-learn.

## Limitations
The dataset is small, with only 25 images per class. Therefore, the reported results should be interpreted as a basic experiment rather than a definitive measure of real-world performance.

## Author
Week 2 Image and Scene Recognition Assignment
