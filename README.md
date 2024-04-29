# Devanagari Script Character Recognition Using Machine Learning

## Introduction

This is a Character Recognition System which I developed for Devanagari Script. The learning model was trained on 92 thousand images (32x32 pixels) of 46 characters, digits 0 to 9 and consonants *ka* to *gya*. The optimal result, 92% accuracy, was obtained using Extremely Randomized Decision Forest Classification algorithm.

## What is Devanagari?

Devanagari is an Indic script and forms a basis for over 100 languages spoken in India and Nepal including Hindi, Marathi, Sanskrit, and Maithili. It consists of 47 primary alphabets, 14 vowels, and 33 consonants, and 10 digits. In addition, the alphabets are modified when a vowel is added to a consonant. There is no capitalization of alphabets, unlike Latin languages.

## What is Machine Learning?

Machine learning is a practical approach for Artificial Intelligence. It uses concepts of Statistics, Probability, Data Science, Computer Algorithms, and Programming. The goal of a machine learning model is to make predictions using data. It is one of the most exciting fields in academic and industrial research.

Machine Learning finds various applications in

- Driverless cars (Google, Tesla)
- Digital Assistants (OK Google, Siri, Cortana)
- Recommendation systems (Amazon, Netflix)
- Spam/Fraud detection (Email, Payment Gateways)
- Computer vision (OCR, Image Transcription)
- Various other automations

## What is Character Recognition?

Character Recognition is the identification of printed characters from an image, a book, a handwritten note, cheques, or letters. It is similar to using a handheld scanner to read a barcode, or reading OMR exam sheets, but it can distinguish between different alphabets.

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

## What's next!

I intend to expand the study by creating or obtaining, the complete dataset, vowels are missing right now. The complete model will then be used to create an application which can read any language in Devanagari script from a book or a handwritten note.

## References

The dataset was originally created by Computer Vision Research Group, Nepal. In a similar study, a student from Kathmandu, Subhigya Nepal used Neural Network on the digits classes, 0 to 9, obtaining an accuracy of 95% (unverified).

## Copying

Devanagari Character Recognition System is a character recognition program for Devanagari Script. Copyright © 2016 Rishi Anand.

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program. If not, see <https://www.gnu.org/licenses/>.

## External Links

[Github Repository](https://github.com/rishianand54/devanagari-character-recognition-system)

[Kaggle Database Repository](https://www.kaggle.com/rishianand/devanagari-character-set)

[Computer Vision Research Group — Website archive](https://web.archive.org/web/20160105230017/http://cvresearchnepal.com/wordpress/dhcd/)

[Subhigya Nepal — blog](http://www.thelacunablog.com/)

[Contact](https://rishianand.me/about/)
