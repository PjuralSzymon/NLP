# NLP Model Trainer

This Python script serves as a versatile tool for training Natural Language Processing (NLP) models, specifically designed for the Speech Commands Data Set v0.01. It enables the exploration of various combinations of preprocessing techniques and neural network architectures. TensorFlow and Keras are utilized for deep learning tasks.

## Description

The script supports the following preprocessing techniques:

- **MFCC (Mel-Frequency Cepstral Coefficients)**
- **Mel Spectrogram**
- **Raw Spectrogram**

And the following recurrent neural network (RNN) models:

- **GRU (Gated Recurrent Unit)**
- **LSTM (Long Short-Term Memory)**
- **SimpleRNN (Simple Recurrent Neural Network)**

## Usage

To use the script, you can run it with the following parameters:

- `--path`: Path to the audio dataset. Default is '../data/train/audio/'.
- `--experiment_name`: Name for the folder containing results. Default is 'model_testing'.
- `--data_limit`: Limit the number of examples per class in the dataset. Default is 100.

For example:

python main.py --path ../data/train/audio/ --experiment_name model_testing --data_limit 100

## Description

This script enables the training of models using different combinations of preprocessing techniques and neural network architectures. The training process is repeated five times with different random seeds for better generalization.

Results, including confusion matrices, training history, and accuracy descriptions, are saved in the './results/' directory. Each experiment has its folder, and within each experiment, there are subfolders for each model and preprocessing technique combination.

## Requirements

Make sure you have the necessary dependencies installed before running the script:

- numpy
- pandas
- tensorflow
- scikit-learn

## License

This project is licensed under the MIT License - see the LICENSE file for details.
