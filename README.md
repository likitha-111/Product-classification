# Product Classification Project

This project focuses on building a multi-class product classification model. It aims to categorize fashion products into different sub-categories based on product images.

## Dataset

The dataset used for this project has been taken from Kaggle:
[Fashion Product Images (Small)](https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-small)

This dataset contains images of fashion products along with their corresponding styles and categories (e.g., gender, master category, sub category, article type).

## Models Used

In this project, we experiment with and compare two different pre-trained deep learning architectures for the classification task:

1. **ResNet18**: A widely-used convolutional neural network architecture known for its residual connections, which help in training deeper networks effectively while avoiding the vanishing gradient problem.
2. **EfficientNet**: A highly efficient family of image classification models that achieve state-of-the-art accuracy while being smaller and faster than many previous models.

## Project Structure

- `product_classifier_training.ipynb`: The main Jupyter Notebook containing the complete workflow including data loading, preprocessing, model definition, training, evaluation, and inference.
- `Accuracy_Comparision.png`: A plot comparing the training/validation accuracy of the models.
- `Confusion_Matrix.png`: A visual representation of the model's classification performance across different product categories.
- `Inference_Time.png`: A chart comparing the inference time (speed) of the used models.

## Setup and Usage

### Prerequisites

The project requires Python and several machine learning and data processing libraries. You can install the necessary dependencies using pip:

```bash
pip install torch torchvision timm pandas scikit-learn pillow
```

### Running the Code

1. Download the dataset from the provided Kaggle link and extract it.
2. Open the `product_classifier_training.ipynb` notebook.
3. Update the data paths in the notebook to point to your local dataset directory.
4. Execute the cells sequentially to prepare the data, train the ResNet18 and EfficientNet models, and compare their results.
5. The trained model weights will be saved (e.g., `efficientnet_product_classifier.pth`) for future inference.

## Evaluation and Results

The results of the experiments are documented within the notebook and the accompanying plots. The project evaluates the models based on:
- **Accuracy**: How well each model correctly classifies the fashion products.
- **Inference Time**: The time taken by each model to predict the class of an image.
- **Confusion Matrix**: To identify which classes the models are confusing with one another.