# ML_Metastatic_Prediction-
Machine Learning Characterization of a Novel Panel for Metastatic Prediction in Breast Cancer

## Background

Metastasis is one of the most challenging problems in cancer diagnosis and
treatment, as its causes have not been yet well characterized. Prediction of
the metastatic status of breast cancer is important in cancer research because
it has the potential to save lives. However, the systems biology behind
metastasis is complex and driven by a variety of factors beyond those that
have already been characterized for various cancer types. Furthermore,
prediction of cancer metastasis is a challenging task due to the variation in
parameters and conditions specific to individual patients and mutation of the
sub-types.

## DataSet

Number of Sample : 202

Number of Metastasis : 101

Number of Non Metastasis : 101

Number of Genes : 54675


## Feature Selection

We selected the data for each gene and separated it by class. 

we got histograms of the values of two separate classes. 

We used the normalized version of the difference of the histograms to decide whether to use that gene.
We select 133 genes from 54675 genes with this method.

for detail 
[Feature_selection.ipynb](https://github.com/melihagraz/ML_Metastatic_Prediction/blob/main/Feature_selection.ipynb)


## Work and Results
we apply tree-based machine learning algorithms for gene expression data analysis in the estimation of metastatic potentials 

Data splitted %80 Training %20 Test

Results of the models

### Decision Tree

```
Classification Report : 
               precision    recall  f1-score   support

           0       0.78      0.72      0.75        25
           1       0.61      0.69      0.65        16

    accuracy                           0.71        41
   macro avg       0.70      0.70      0.70        41
weighted avg       0.72      0.71      0.71        41
```

### Extremely Randomized Trees

```
Classification Report : 
               precision    recall  f1-score   support

           0       0.80      0.96      0.87        25
           1       0.91      0.62      0.74        16

    accuracy                           0.83        41
   macro avg       0.85      0.79      0.81        41
weighted avg       0.84      0.83      0.82        41

```

###  Gradient Boosting

```
Classification Report : 
               precision    recall  f1-score   support

           0       0.86      0.96      0.91        25
           1       0.92      0.75      0.83        16

    accuracy                           0.88        41
   macro avg       0.89      0.85      0.87        41
weighted avg       0.88      0.88      0.88        41
```

for detail 
[Training_and_evaluation.ipynb](https://github.com/melihagraz/ML_Metastatic_Prediction/blob/main/Training_and_evaluation.ipynb)




