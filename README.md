# PahariLI
Text corpus and ML models for Pahari languages identification

This repository contains the text corpus and models developed for identification of four Pahari/Northern Indo-Aryan languages languages - Dogri, Garhwali, Kumaoni and Nepali.
The text corpus consists of two data files:

- train.txt: It consists of 44,014 labeled sentences.
- test.txt: It consists of 11,004 labeled sentences.

Every sentence is labeled with the ISO 639-3 code of the corresponding language.

For language identification, word and character based n-gram models fitted on train data are used to train Multinomial Naive Bayes and Support Vector Machines. Hyperparameters are tuned using 5-fold cross-validation approach. The resulting models are evaluated on the test data.
