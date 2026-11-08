
# AI-Based Crop Disease Detection Using Deep Learning and Explainable AI

## Project Overview
This case study uses deep learning to classify plant leaf images into different healthy and diseased categories. The project uses MobileNetV2 transfer learning to recognize visual patterns in leaf images and Grad-CAM to visualize the image regions that influence predictions.

## Problem Statement
Plant diseases can reduce crop quality and agricultural yield. Manual identification of diseases may take time and require experience. This project explores an image-classification approach that can help identify possible plant diseases from leaf images.

## Dataset
**PlantVillage Dataset**

- 38 classes in the standard dataset
- Plant leaf images representing different plant health and disease categories
- Training and testing subsets used for model development and evaluation

## Methodology
1. Load the PlantVillage dataset.
2. Resize images to 160 × 160 pixels.
3. Preprocess images for MobileNetV2.
4. Use a pretrained MobileNetV2 model for feature extraction.
5. Train a softmax classification layer.
6. Evaluate the model using test accuracy, test loss, and a confusion matrix.
7. Use Grad-CAM to visualize image regions influencing predictions.

## Machine Learning Model
- MobileNetV2
- Transfer learning
- Softmax classifier
- Grad-CAM explainability

## Technologies Used
- Python
- Google Colab
- TensorFlow
- TensorFlow Datasets
- Scikit-learn
- NumPy
- Pandas
- Matplotlib
- Seaborn

## Results

The following results were obtained from the completed notebook:

| Metric | Result |
|---|---:|
| Number of classes | 38 |
| Epochs completed | 3 |
| Test examples | 10,861 |
| Test accuracy | 95.37% |
| Test loss | 0.1364 |
| Correct predictions | 10,358 |
| Incorrect predictions | 503 |

## Explainable AI
Grad-CAM generates a heatmap highlighting image regions that influence a selected class prediction. This helps inspect the model's behavior but does not guarantee that a prediction is correct.

## Limitations
The model was evaluated on the PlantVillage dataset. Real-world field images may differ in lighting, background, camera quality, and disease severity. Further testing on independent field images is needed before practical use.

## How to Run
1. Download `CLA3_Crop_Disease_Classification.ipynb`.
2. Open Google Colab.
3. Upload the notebook.
4. Run the cells in order.
5. Review the evaluation metrics, confusion matrix, sample predictions, and Grad-CAM heatmap.

## Author
**Name:** Y. Hemsaicharan  
**Roll Number:** AP24110010374
