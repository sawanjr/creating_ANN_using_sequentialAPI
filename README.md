# Side Effect Prediction using TensorFlow and scikit-learn

This repository contains a machine learning model built using TensorFlow and scikit-learn to predict the likelihood of side effects from an experimental drug based on individual's age. The model is designed to distinguish between two groups: individuals under 65 years old and those who are 65 years or older.

## Requirements

- Python 3.x
- TensorFlow
- scikit-learn

Install the required packages using the following command:
pip install tensorflow scikit-learn

## Dataset

The experimental drug was tested on a total of 2100 participants, with half under 65 years old and half 65 years or older. Approximately 95% of patients in both groups experienced side effects.

## Usage

1. Clone this repository:


git clone [https://github.com/yourusername/side-effect-prediction.git](https://github.com/sawanjr/creating_ANN_using_sequentialAPI.git)
cd side-effect-prediction


2. Open the provided Python script `side_effect_prediction.py` in your preferred code editor.

3. Run the script to build and train the machine learning model.


python side_effect_prediction.py


## Model Architecture

The TensorFlow model consists of three layers:
- Input layer with 16 units and ReLU activation
- Hidden layer with 32 units and ReLU activation
- Output layer with 2 units and softmax activation

The model is compiled with the Adam optimizer using a learning rate of 0.0001 and sparse categorical cross-entropy loss. It is then trained on the scaled training samples for 30 epochs.

## Model Evaluation

After training, the model's performance can be evaluated using the validation split. A comparison between training accuracy and validation accuracy helps to understand whether the model is overfitting or underfitting.

## Testing

The model's predictions are tested on a separate set of data (test samples). The test samples are similarly generated based on age groups, and then they are scaled using the MinMaxScaler. The model predicts the likelihood of side effects for each test sample.

## Conclusion

This project demonstrates the use of TensorFlow and scikit-learn to build a machine learning model for side effect prediction based on age groups. The model's performance is evaluated and tested, providing insights into its generalization capabilities.

Feel free to explore the code and experiment with different parameters to improve the model's accuracy and performance.

For questions or suggestions, please contact [sawanrawatjr10@gmai.com](sawanrawatjr10@gmai.com).
