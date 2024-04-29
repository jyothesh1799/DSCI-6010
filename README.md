# Devanagari Script Character Recognition 

## Introduction

This is a Character Recognition System which I developed for Devanagari Script. The learning model was trained on 92 thousand images (32x32 pixels) of 46 characters, digits 0 to 9 and consonants *ka* to *gya*. The optimal result, 92% accuracy, was obtained using Extremely Randomized Decision Forest Classification algorithm.

## What is Devanagari?

Devanagari is an Indic script and forms a basis for over 100 languages spoken in India and Nepal including Hindi, Marathi, Sanskrit, and Maithili. It consists of 47 primary alphabets, 14 vowels, and 33 consonants, and 10 digits. In addition, the alphabets are modified when a vowel is added to a consonant. There is no capitalization of alphabets, unlike Latin languages.

## What is Character Recognition?

Character Recognition is the identification of printed characters from an image, a book, a handwritten note, cheques, or letters. It is similar to using a handheld scanner to read a barcode, or reading OMR exam sheets, but it can distinguish between different alphabets.

## 4.1 Install Dependencies:

1. Pandas
2. Numpy
3. random
4. datetime
5. Tensorflow
6. OS
7. Seaborn
8. Matplotlib

Anaconda and jupyter notebook is a better way to install dependencies 



## [Technical] Project Walkthrough

A sample of the dataset is analyzed using various algorithms, and their scores and computational costs are compared.

| Algorithm              | Accuracy (in percent) | Total Time (in seconds) |
| -----------------------| ---------------------:| -----------------------:|
| RidgeClassifier        | 42.3384               | 00.712410               |
| BernoulliNB            | 51.2742               | 00.168973               |
| GaussianNB             | 39.6972               | 01.411730               |
| ExtraTreeClassifier    | 31.1093               | 00.109071               |
| DecisionTreeClassifier | 36.5119               | 04.080331               |
| NearestCentroid        | 53.0247               | 00.127525               |
| KNeighborsClassifier   | 72.1442               | 36.413726               |
| ExtraTreesClassifier   | 57.4804               | 00.563712               |
| RandomForestClassifier | 54.3047               | 00.932044               |

Using the above table, K Nearest Neighbors Classification, Extremely Randomized Decision Forest Classification and Random Forest Classification algorithm are selected. A Grid Search is performed to obtain optimum parameters and scores of these algorithms and compare their performance.

![K Nearest Neighbors Classification Algorithm Grid Search](plots/knn.png)

![Extra Trees Classification Algorithm Grid Search](plots/extra-trees.png)

![Random Forest Classification Algorithm Grid Search](plots/random-forests.png)

Extra Trees Classification algorithm is used to plot a Learning Curve.

![Learning Curve with Extra Trees Classification Algorithm](plots/learning-curve.png)

## Conclusions

The final result, using Extremely Randomized Decision Forest Classification Algorithm with 256 trees gives an accuracy score of 92%.


## References

The dataset was originally created by Computer Vision Research Group, Nepal. In a similar study, a student from Kathmandu, Subhigya Nepal used Neural Network on the digits classes, 0 to 9, obtaining an accuracy of 95% (unverified).


