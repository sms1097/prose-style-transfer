# Formality Transfer
This repo contains all of the work for my senior project and class project for CS 880. <br>
In order to run this code authorization from Yahoo to access the L6 corpus is needed 
and authorization must be shown to Joel Tetreault. Full details can be found [here](https://github.com/raosudha89/GYAFC-corpus)

## CS 880
### [Vanilla Encoder-Decoder](https://github.com/sms1097/formality-transfer/blob/master/supervised/Baselines/Vanilla%20Encoder%20Decoder.ipynb)
This is a basic Encoder-Decoder model with no attention.

### [RNN with Global Attention](https://github.com/sms1097/formality-transfer/blob/master/supervised/Baselines/Global%20Attention%20Model.ipynb)
This is the global attention implementaiton.

### [CRF POS with Global Attention](https://github.com/sms1097/formality-transfer/blob/master/supervised/Multi-Encoder%20RNN/CRF%20POS%20Concat.ipynb)
This is the parallel encoder model with global attention. The CRF POS model was trained in [this](https://github.com/sms1097/formality-transfer/blob/master/supervised/Multi-Encoder%20RNN/POS%20Generation.ipynb) notebook.

## Senior Project
### Transformer Based Models
All models trained using OpenNMT-tf are configured using a data.yaml file, a bash script for running the model, and a translate script. The multi-column encoder models involve a special transformer model that was written on top of the existing transformer model inside of the library. 

#### [Custom Transformer](https://github.com/sms1097/formality-transfer/blob/master/supervised/Baselines/Transformer%20Model.ipynb)
As mentioned in the paper this model was not used since the requirements for training were too great. 

#### [ONMT Transformer](https://github.com/sms1097/formality-transfer/tree/master/supervised/Baselines/onmt-transformer)
This is the folder that contains configuration for the  baseline transformer model. 

#### [Formality Discrimination](https://github.com/sms1097/formality-transfer/tree/master/semi-supervised/Formality%20Discrimination)
This folder contains all fo the work done on formaltiy transfer. [Formality Discrimination](https://github.com/sms1097/formality-transfer/blob/master/semi-supervised/Formality%20Discrimination/Formality%20Discrimination.ipynb) is the notebook where all the data was split up before feeding into google translate. [Formality Classifier](https://github.com/sms1097/formality-transfer/blob/master/semi-supervised/Formality%20Discrimination/Formality%20Classifier.ipynb) is where the classifier was trained to be able to detect formal sequences and the augmented training set was determined. The folder [formality-discrimination](https://github.com/sms1097/formality-transfer/tree/master/semi-supervised/Formality%20Discrimination/formality-discrimination) contains the OpenNMT-tf model configuration.

#### [Backtranslation](https://github.com/sms1097/formality-transfer/tree/master/semi-supervised/backtranslation)
Two folders are here: one for the back translation model and one for the transformer with the augmented data

#### [POS Assisted](https://github.com/sms1097/formality-transfer/tree/master/supervised/Multi-Encoder%20Transformer/crf-pos/transformer-crf)
Multi-column encoder with sequences and POS.

#### [Rule-Assisted](https://github.com/sms1097/formality-transfer/tree/master/supervised/Multi-Encoder%20Transformer/rule-assisted)



