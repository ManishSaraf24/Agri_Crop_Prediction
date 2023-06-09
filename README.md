# Agriculture Crop Prediction

This project aims to predict agricultural crop yields using machine learning algorithms,
specifically an Artificial Neural Network (ANN) model. The goal is to provide farmers with accurate predictions of crop to produce,
which is suitable for thier environmental conditions.

## Dataset

The dataset used for this project consists of historical agricultural data,
including information such as temperature, soil pH, humidity , Nitrogen , Phosphourus , Pottassium  and Rainfall. Each data entry represents a specific combination of these factors for a particular crop. There is a large data containing of various crops such rice , banana , grapes , apple , mothbeans etc.

## Methodology
We took dataset as mentioned above and applied machine learning algorithms on it such random forest, decision tree , K-means clustering and KNN etc.to check accuracy of models and to choose best fit model for prediction.After getting highest accuracy of random forest we just applied it on our dataset ,we split dataset into two parts train and test.We got 99.7 accuracy for random forest so we moved with it and trained our model accordingly. It predicts accurate results now on giving input of temperature , pH , nitrogen , phosphorous , rainfall , humidity etc .


## Dependencies

To run this project, you will need the following dependencies:

- Python
- NumPy
- Pandas
- Scikit-learn
- ANN 
- Random Forest Classifier
- Streamlit (GUI)
- few algorithms like decision tree,K-means clustering, KNN etc to check accuracy 

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/agriculture-crop-prediction.git
   ```

2. Install the required dependencies:

   ```bash
   pip install numpy pandas scikit-learn keras tensorflow
   ```

## Usage

1. Navigate to the project directory:

   ```bash
   cd agriculture-crop-prediction
   ```

2. Prepare the dataset:

   - Place the dataset file in the `data` directory.
   - Modify the `config.py` file to specify the dataset filename, as well as any other relevant configurations.

3. Train the ANN model:

   ```bash
   python train.py
   ```

   This command will train the ANN model on the provided dataset. The trained model will be saved in the `models` directory.

4. Make predictions:

   ```bash
   python predict.py
   ```

   By running this command, the trained ANN model will be loaded, and predictions for crop yields will be generated based on the provided input data. The predicted results will be displayed in the console.

## Configuration

The `config.py` file contains various configurations that can be customized:

- `data_filename`: The filename of the dataset file.
- `train_test_split`: The ratio of training data to testing data during model training.
- `num_epochs`: The number of epochs to train the ANN model.
- `batch_size`: The batch size used during model training.
- `learning_rate`: The learning rate for the optimizer used during model training.
- `hidden_layers`: A list representing the number of neurons in each hidden layer of the ANN model.
- `activation`: The activation function used in the hidden layers of the ANN model.
- `output_activation`: The activation function used in the output layer of the ANN model.



## Contributing

If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Implement your changes.
4. Test thoroughly.
5. Submit a pull request explaining the changes you have made.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use and modify it for your own purposes.

## Acknowledgments

We would like to acknowledge the following resources that were helpful in the development of this project:

- [Scikit-learn documentation](https://scikit-learn.org/stable/documentation.html)
- [Keras documentation](https://keras.io/)
- [TensorFlow documentation](https://www.tensorflow.org/api_docs)
- [Python documentation](https://docs.python.org/3/)

Thank you for using this agriculture crop prediction project. If you have any questions or feedback, please don't hesitate to reach out.
