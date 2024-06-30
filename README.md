# Breast-Cancer-Prediction

## Overview 
Breast Cancer is the most common type of cancer amongst women in the world. Breast cancers are caused when malignant(cancer) cells form in the tissues of the breast. These cells usually form tumors that can be seen via X-ray or felt as lumps in the breast area.

This project aims to build a predictive model to diagnose breast cancer using machine learning techniques. The goal is to assist medical professionals in making accurate and timely decisions by predicting whether a tumor is malignant or benign based on input features. The model is trained using neural networks taken from a dataset in Kaggle and outputs whether the tumor is malignant or benign.

### Dataset
The dataset used in this project is the [breast_cancer_data](https://www.kaggle.com/datasets/yasserh/breast-cancer-dataset) dataset from Kaggle. It includes 30 features defining various measurements of the ingrown tumor and the diagnosis (malignant or benign).
To continue with the model training process, the dataset is analyzed and cleaned using numpy, pandas and matplotlib.

### Features

   * Radius (mean of distances from center to points on the perimeter)
   * Texture (standard deviation of gray-scale values)
   * Perimeter
   * Area
   * Smoothness (local variation in radius lengths)
   * Compactness (perimeter^2 / area - 1.0)
   * Concavity (severity of concave portions of the contour)
   * Concave points (number of concave portions of the contour)
   * Symmetry
   * Fractal dimension ("coastline approximation" - 1)

### Preprocessing the data

Data is splitted using train-test-split in scikit-learn.

60% of the data is used for training the neural network model, while 20% is used as cross-validation data and other 20% is used as test data. Spliiting of data in this way allows for an accurate assessment of the model's ability to generalize to new samples.

Data is standardized using StandardScaler module in scikit-learn.

### Training and Evaluating the model

The project utilizes a simple neural network architecture to build the model using tensorflow. A sequential model is implemented with 3 dense layers. Layer 1 contains 16 units with a 'relu' activation. The hidden layer takes 16 units form the previous layer as the input and outputs 16 units. The output layer outputs 2 units with 'sigmoid' activation. 

The model implies 97% accuracy for test data. A confusion matrix is created to compare the predicted labels against th actual labels. These metrics provide insights into the model's ability to correctly classify malignant and benign breast cancer samples.

## Dependencies

 * pandas: Data cleaning and data analysis
 * numpy: Numerical computing
 * matplotlib:  Data Visualization
 * tensorflow: Build and train the neural network model
 * scikit-learn: Data modeling

 ## How to run the model

 ### 1. Prerequisites

 Make sure you have the following installed:

- [Python](https://www.python.org/downloads/) (version 3.6 or higher)
- [Git](https://git-scm.com/)

### 2. Clone the Repository

```bash
git clone https://github.com/your-username/Breast-Cancer-Prediction.git
cd Breast-Cancer-Prediction
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```
### 4. Download the model

Download the 'model.h5' file in the same directory.

### 5. Run the Jupyter Notebook

Launch Jupyter Notebook and open the .ipynb file to run the model:

```bash
jupyter notebook
```

Navigate to the notebook file [cancer_prediction.ipynb](cancer_prediction.ipynb) and open it in the browser and run the notebook cells sequentially. 

## Conclusion

This project offeres a practical solution for classifying breast cancer tumor samples as malignant or benign using a basic neural network model. It includes data collection, preprocessing, data visualization, model training and model evaluation. This project can be further developed as an end-to-end project which predicts breast cancer risk using a web app.


### 
Feel free to explore the code. If you have any questions or feedback, please reach out at [rmovinya10@gmail.com](mailto:rmovinya10@gmail.com)




