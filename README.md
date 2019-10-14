#### Wine-project

##Desription
>I took Data set about wine. Wine has same atributes(11) and label y(quality of wine on scale 3 to 8). Problem is multiclassification, where I want to predict if wine for these attributes will be good quality (7,8), bad quality(3,4) or middle quality(5,6). 

>At first I want to try solve binnary classification (If wine has good quality (7,8) or other quality). For that reason I created special column 'Qgood' with values 1 godd quality wine(7,8) and 0 others. 

>At the beginning of the project I was interested about dependency between atributes and results. I wanted also see dependency between the atributes. My expectation are, that if two attributes have high correlation between each other, that one of these atributes can be meanningless and can be removed from atributes. This atribute can be only diffrent description of corralted atribute. If my results and one of the atribute have high corellation, than I expect that this atribute is significant in my model. 

###My progress is following:
* 1. Item 1 Split data na training data and testing data
* 1. Item 2 Scaled data
* 1. Item 3 I tryed to use diffrent models with interest which kind of results they can show. 
   * Item 3a **k_nearest Neighbors classifier** I tryed to visualise this model with diffrent number of neighbours. I did it for my imagination, to could see, when it shows best results. It looks that best results we will get when model is calculated from 100 neighbours. 
   * Item 3b **Logistic regresion** This model is interesting for me because I wanted to play with probability of results.I expect that probability is set up for 0,5. I wanted to set up pst|1=0.7 and see if my confusion matrix could offer me better results. 
   * Item 3c **Decision Tree classifier** I visualise the results but I don't expect that this model can bended some how. I only know that I can set up the depth of the tree. Maybe I will try it later. 
   * Item 3d **Linear suport vector machine classifier** For my overview, I set up diffrent values for gamma.
   * Item 3e **Dummy classifier** - I created dummy classifier whith strategy='most-frequent' for my overview of score how it would look when all my predictions would have result most frequent class.  
* Item 4 I visualise evaluation matrics and classifiacation report for logistic regression. 
* Item 5 I work with predict_proba to could see with how probability occurs my predict value. Than I shows the results which have difference between y_test value and predicted value. Last number in every line is pst|1. If pst>0,5, predicted value will be 1. 
* Item 6 At the end I am playing with Precision recall curves. 
