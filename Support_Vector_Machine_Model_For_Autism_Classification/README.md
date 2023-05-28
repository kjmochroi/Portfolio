## Autism Classification Using Support Vector Machine Model and the AQ-10 Survey   

### By KJ MoChroi
#### April 2023

For this project I used data collected from a ten-question survey called the Autism Quotient - 10 Questions (AQ-10) to create a binary support vector machine (SVM) classification model that can determine whether an adult should be referred to a professional clinician for the possible diagnosis of autism spectrum disorder. This investigation can be used to determine whether this short questionnaire is adequate in identifying such adults or whether a more thorough approach is needed.  

The data consists of 20 variables including some demographic information, the responses to the 10 questions on the survey, and the binary target feature. The demographic information was used during the exploratory analysis to better understand which populations may be underrepresented in the study. However, when it came time to train the model these features were dropped and only the 10 features that were responses to the questionnaire were included in training. The demographic features were the only training features to contain missing information so when they were dropped, we simultaneously cleaned the dataset if missing values. The target feature is a binary categorical variable that has just over 500 instances of non-ASD and just under 200 of ASD. All of the training features had some predictive power over the target feature, with Pearson's correlation coefficients ranging from 0.24 to 0.64 between training features and the target class.

After cleaning the training data, I performed hyperparameter tuning using the gridsearch technique. With those optimized parameters I was able to train an SVM model with an average of 99.4% accuracy across the 5-fold cross-validation method I used to validate the model. This is significantly better than the 70% accuracy one would obtain with the null model that predicts non-ASD for every instance.

In terms of accuracy, this model is a large improvement to the current scoring method of simply summing the result of each question and comparing that total to a benchmark. While this is a large improvement to the current scoring method, there are some ethical considerations we should make when reviewing this model. It is likely that this model inhereted some of the cultural biases of the medical community who did the original diagnostics to determine which people had ASD and which didn't.

This folder contains a Jupyter Notebook file with the model, the original dataset and data description, as well as a white paper, and a presentation of my findings.
