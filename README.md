# Ensemble-UNet-Enhancing-Brain-Tumor-Segmentation

In this project, we employ an ensemble learning approach by integrating four pre-trained networks: MobileNet, DeepLabV3+, ResNet, and DenseNet as the encoders within the U-Net architecture. Our experimental evaluation showcases promising results, achieving an Intersection over Union (IoU) score of 0.86, a Dice Coefficient (DC) of 0.92, and an accuracy of approximately 0.99. These results emphasize the effectiveness of our proposed U-Net-based architecture and ensemble learning approach for accurate brain tumor segmentation.

# Accuracy Metrics

This section outlines the accuracy metrics used to evaluate the performance of the segmentation model in this project. These metrics play a crucial role in assessing how well the model's predictions align with the ground truth data.

## Dice Coefficient (dice_coef)

The Dice Coefficient is a widely used metric for quantifying the similarity between predicted and ground truth masks. It is computed using the following formula:

Dice Coefficient (dice_coef) = (2 * intersection + smooth) / (sum(y_true) + sum(y_pred) + smooth)

Where:
- `y_true` represents the ground truth mask.
- `y_pred` represents the predicted mask.
- `smooth` is a smoothing factor set to 100 to prevent potential division by zero errors.

## Dice Coefficient Loss (dice_coef_loss)

The Dice Coefficient Loss is the negation of the Dice Coefficient and serves as a loss function for training the segmentation model.

## Intersection over Union (IoU or jac)

The Intersection over Union, also known as the Jaccard Index, gauges the overlap between predicted and ground truth masks. It is calculated as follows:

IoU (Intersection over Union) = (Intersection + Smooth) / (Sum(y_true) + Sum(y_pred) - Intersection + Smooth)

## Jaccard Distance (jac_distance)

The Jaccard Distance measures the dissimilarity between predicted and ground truth masks and is the negative counterpart of the IoU

# DATASET
The dataset used in our research is the LGG segmentation dataset. It comprises MR (Magnetic Resonance) images, each containing three RGB channels, and all images are presented in .tif format with a size of 256x256 pixels



