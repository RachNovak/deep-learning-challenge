# deep-learning-challenge
Challenge21_deep-learning-challenge

# README.md

This README file provides an overview of the code and steps involved in preprocessing and training a deep neural network model for a charity classification task.

## Preprocessing

In this section, the dependencies are imported, and the charity data is imported and read from the provided CSV file. The non-beneficial ID columns, 'EIN' and 'NAME', are dropped from the dataset. The number of unique values in each column is determined, and binning is performed on the 'APPLICATION_TYPE' and 'CLASSIFICATION' columns. Categorical data is converted to numeric using one-hot encoding with `pd.get_dummies`. The preprocessed data is then split into features (X) and target (y) arrays, and further split into training and testing datasets. The data is also scaled using the StandardScaler.

## Compile, Train, and Evaluate the Model

In this section, the deep neural network model is defined using the Keras Sequential API. The model architecture includes multiple dense layers with specified number of hidden nodes. The model is compiled with the binary_crossentropy loss function, Adam optimizer, and accuracy as the metric. The model is trained on the scaled training data and evaluated using the scaled testing data. The model's loss and accuracy are printed.

## Exporting the Model

In this final step, the trained model is saved in the HDF5 format for future use.

This README.md file provides an outline of the code and steps involved in preprocessing and training the deep neural network model for the charity classification task. For more details, refer to the source code file.
