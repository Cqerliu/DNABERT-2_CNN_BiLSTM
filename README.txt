Dataset Description
This dataset contains multiple Excel worksheets, primarily used for training, validation, and testing machine learning models. Below is a detailed description of the dataset.

Dataset Structure:
The dataset contains the following worksheets:
Train: The training set used to train the model.
Dev: The development (validation) set used to evaluate the model's performance during training.
Test: The test set used to evaluate the model's final performance.

File Description:
Train.xlsx: Contains the data required for training the model. This file includes the training samples used to train the model.
Dev.xlsx: Contains the data required for model validation. This file is used to evaluate the model's performance during training.
Test.xlsx: Contains the data required for model testing. This file is used to evaluate the model's final performance after training.

Fine-Tuning Strategies
This study employs three different fine-tuning strategies, each stored in separate folders. The training and testing conditions for each strategy are as follows:
Individual Learning: Model training and testing were conducted on the hearing loss dataset.
Cross-Disease Training: Model training was conducted on the breast cancer and cervical cancer datasets, with testing on the hearing loss dataset.
Global Training: Model training was conducted on all known human promoter datasets, with testing on the hearing loss dataset.