# Pima-diabetes prediction 💉

![image](https://drive.google.com/uc?export=view&id=1HHiisNmsBIlk7D1kPnYTr4N5Xl2wKx7O)

[link for the presentation](https://drive.google.com/file/d/1M_7U--7h1u55vca3boF1HnhnKrhpDeJg/view?usp=sharing)

## **Project motivation**

In these project we want to predict whether or not a patient has diabetes, based on certain diagnostic measurements included in the dataset.

## **The Dataset**
This dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases. [Kaggle](https://www.kaggle.com/uciml/pima-indians-diabetes-database) 

### **Data Description**
The datasets consists of several medical predictor variables and one target variable, Outcome (1 - diabetes, 0 = no diabetes)

## **Analaysis Plan** 📈

Here we want to predict whether ot not the patient has diabetes. the target will be 1 or 0 , so it is a supervised binary classification problem. the follwing steps will be followed:


1.   Cleaninng Data 🧹
2.   Explarotaory data analysis to discover an intitial insights.🔍
3.   Select the suitable algorithm (KNN, logestic regression, Tree classification,svm)
4.   Fit the data to the model, fine tune, evaluate and validate.


## **Summary**

The project aimed to investigate the potential to develop a predictive model to predict  if a patient have a diabetes or not using features collected from 
the national Institute of Diabetes and Digestive and Kidney Diseases, from 758 females.these data was collected before 23 year ( 1998).the data also unbalanced, it have 32% diabetic females  and 68% healthy females.

The results from the model
can then be used to help identify if the patients have a diabetes or not. a voting estimator ( SVM and logistic regression)
was developed that achieved a weighted ROC AUC Score on the validation set of 0.83.
This model has potential but need to be improved more, maybe collecting more data and adding more features like if there is another background diseases,  smoking or not, the economic situation etc.

To improve the model more, we should focus on collecting data for females who have a glucose level less than 140 and have diabetes, because we noticed that the model didnt predict well these category and have just an accuracy of 21.2% (can predict just 21.2% from these category). in our dataset there was almost 190 cases for females who have glucose levels less than 140  after the glucose tolerance test and have diabetes. 
This will help to build classifiers that are better at  predicting the
diabetic females and decrease the flase negative ratio.

The importances of the features were determined using information extracted from each model in the voting estimator( the SVM model and the logistic regression).
By the **logistic regression model**, the most important feature was the 
Diabetes **Peidegree function** which is "a synthesis of the diabetes mellitus history in relatives and the genetic relationship of those relatives to the subject.”, while by the **svm model** the most important feature was the **glucose level**, it is right because by the glucose tolerance test, doctors can classifiy the patients if she have a diabetes or not , so if he have glucise level higher than 140 she will be classified as diabetic.

we checked also the weighted f1-score which is the harmonic average of the precision and the accuracy, it was between 76% to 80% in the training and the testing set respectively.

At the end, these model have a potential but we need to add more data and features to improve it more. 


**Note :** 


1- The data also is old from 1998, so we dont really know how much it is accurate. <br>
2- the data is just from female participants so in the machine learning we will just predict the dibetes for the females . 
the data also is so small ,we dont have a lot of records to predict and make a generalization.<br>
3- In the data there is no id for each participant so we could not know if there is a duplicate or if there is some participnats who make the test two times. 

