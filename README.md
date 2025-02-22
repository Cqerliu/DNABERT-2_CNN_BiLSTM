# DNABERT-2_CNN_BiLSTM

DNABERT-2_CNN_BiLSTM, by integrating Convolutional Neural Networks (CNN) and Bidirectional Long Short-Term Memory (BiLSTM) into the BERT model, enhances the ability to extract local features of gene sequences and capture long-range dependencies, thereby improving the predictive analysis of promoters associated with hearing loss.

## Model Description
In this project, we designed and trained five model variants based on BERT, combined with different feature extraction modules, aiming to improve gene promoter prediction performance. The models are described as follows:

1. **DNABERT-2_BASE**: The base model that encodes gene sequences using BERT without any additional feature extraction modules.
   
2. **DNABERT-2_CNN**: This model incorporates Convolutional Neural Networks (CNN) to extract local features from gene sequences, improving the model's ability to capture short-range dependencies.

3. **DNABERT-2_BiLSTM**: This variant adds Bidirectional Long Short-Term Memory (BiLSTM) networks to the BERT model, enhancing the ability to model long-range dependencies in gene sequences, especially useful for capturing distant relationships.

4. **DNABERT-2_CNN_BiLSTM(MAX)**: This model combines CNN and BiLSTM with max pooling layers to optimize feature extraction, improving sensitivity to local features and long-range dependencies.

5. **DNABERT-2_CNN_BiLSTM(Avg)**: Similar to DNABERT-2_CNN_BiLSTM(MAX), but uses average pooling layers to balance the importance of features, enhancing model robustness.

## File Description

- **model.rar**: This file contains the original code and run instructions for all five models.
  - The archive includes scripts for training and validating the five models, along with detailed instructions for running each model to facilitate reproducibility.

- **sample_data**: A sample dataset is provided for running and testing the models.
  - The dataset contains gene sequences relevant to the promoter prediction task, with sequence lengths of 300 bp and 600 bp, which can be used for training and validating the models.


- **raw_data**: This folder contains the raw data used for model training and testing.
  - It includes Excel worksheets with the following datasets:
  -Train: The training set used to train the model.
  -Dev: The development (validation) set used to evaluate the model's performance during training.
  -Test: The test set used to evaluate the model's final performance.
  -These datasets include hearing loss-related gene promoter sequences, as well as additional sequences from other diseases (e.g., breast cancer and cervical cancer) to support cross-disease training.

## Running Instructions
1. Extract the `model.rar` file.
2. Follow the running instructions provided in each model folder to set up the environment and run the training or testing scripts.
3. Use the dataset provided in the `sample_data` folder to train and test the models.
4. For the raw data, refer to the raw_data folder to access the relevant training, validation, and test sets required for fine-tuning the models.
