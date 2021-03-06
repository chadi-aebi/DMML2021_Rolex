# DMML2021 - Team Rolex

## Project description
It was asked to us to create a model that could help to predict the difficulty of a french text.

## Team members
- Paula Heess
- Chadi Aebi
- Antoine Hassler
- Imène Ksibi

## How we proceed

In the Notebook ["Notebook_Rolex.ipynb"](https://github.com/chadi-aebi/DMML2021_Rolex/blob/main/code/Notebook_Rolex.ipynb) we will proceed as follows:

First we prepare the notebook by importing essential methods and components for text analytics. Then we will start with some preparations such as building a tokenizer with different possible features to apply this later in the classification.

Subsequently, we start the text analytics divided by the different classifiers starting with a baseline calculation.
Each classifier section starts with a classification without any data preprocessing or other features. Then we tune the hyperparameters for the classifier to find the best parameters. After that, we train models that also implement the preprocessing of data, we try word embeddings and in the end we try out dimensionality reduction and standardisation.

The notebook has the following chapters:


For preparation:
*  Preparation to start working - import necessary methods etc.
*  Further preparation for classification

Testing different classifiers:
* Baseline calculation
* Logistic Regression
* kNN Classifier
* Decision Tree
* Random Forests
* Linear Support Vector Classification

After applying different classifiers we got the following outcome for each classifier without doing any preprocessing or hyperparameter tuning:


|       | Logistic regression |      kNN   |  Decision Tree  |     Random Forests | Linear SVC   |
| ----------- | ----------- | ----------- | ----------- | -----------   | ----------- | 
| Precision      |  0.4578  |  0.3823  |  0.2932  |  0.3801  |  0.4565  |
| Recall   |  0.4595  |  0.3137 |  0.2982  |  0.3838  |  0.4604  |
| F1-score    |  0.4554  |  0.2913  |  0.2944  |  0.3690  |  0.4557  |
| Accuracy   |  0.4604  |  0.3156  |  0.2990  |  0.3854  |  0.4615  |

And we got the following outcome for each classifier with processing and hyperparameter tuning:

|       | Logistic regression |      kNN   |  Decision Tree  |     Random Forests | Linear SVC   |
| ----------- | ----------- | ----------- | ----------- | -----------   | ----------- | 
| Precision      |  0.4899  |  0.3392  |  0.3392  |  0.3887  |  0.4771  |
| Recall   |  0.4927  |  0.3273 |  0.3273  |  0.3912  |  0.4812  |
| F1-score    |  0.4899  |  0.3224  |  0.3224  |  0.3777  |  0.4776  |
| Accuracy   |  0.4938  |  0.3281  |  0.3281  |  0.3927  |  0.4833  |


Link to the youtube video: https://www.youtube.com/watch?v=aIEJij_x8Hc

