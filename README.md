# DiabetesPredection-Machine-Learning
Abstract: 
Diabetes Prediction Using Machine Learning 
Now a days Diabetes is a very common disease in all over the world of all age groups. To diagnose diabetes, a physician has to analyze many factors, data obtained from patients and has to take expert decisions that are very critical. 

But using Machine Learning technique it can be easily diagnose. In this paper we are going to discuss how to use Machine Learning to predict Diabetes. The prediction will predict whether a patient has a diabetes or not. We have used ‘K-Nearest Neighbors’ (KNN) machine learning algorithm for this work. We also measure the Accuracy of K-NN the algorithm and also compare it with another algorithm that is Decision Tree algorithm. Algorithms are works with python Machine learning modules like pandas, sklearn, matplotlib, Seaborn, numpy etc.

 Data: 
A dataset is use to analysis data and make a prediction. The dataset is also needed to train and test the algorithm. The dataset will be in csv form. The dataset we have used here is originally from the ‘National Institute of Diabetes and Digestive and Kidney Diseases’. The objective of the dataset is to diagnostically predict whether or not a patient has diabetes, based on certain diagnostic measurements included in the dataset. In this dataset, all patients here are females.   
The datasets consist of several medical predictor variables and one target variable, ‘Outcome’. Predictor variables includes the number of pregnancies the patient has had, their BMI, insulin level, age, and so on. The diabetes dataset consists of 768 data points, with 9 features each. 

The 9 variables and it’s meanings: 
Pregnancies: Number of times pregnant 
Glucose: Plasma glucose concentration a 2 hours in an oral glucose tolerance test 
BloodPressure: Diastolic blood pressure (mm Hg) 
SkinThickness: Triceps skin fold thickness (mm) 
Insulin: 2-Hour serum insulin (mu U/ml) 
BMI: Body mass index (weight in kg/(height in m)²) 
DiabetesPedigreeFunction: Diabetes pedigree function 
Age: Age (years) 
Outcome: Output variable (0 or 1) 

ALGORITHM K-NN: 
The k-NN algorithm is arguably the simplest machine learning algorithm. Building the model consists only of storing the training dataset. To make a prediction for a new data point, the algorithm finds the closest data points in the training dataset — its “nearest neighbors.” 

 “Outcome” is the feature we are going to predict, 0 means No diabetes, 1 means diabetes. Of these 768 data points, 500 are labeled as 0 and 268 as 1: 
 
 K-Nearest Neighbors Apply: 
Visualization of training and test data accuracy: 
 
As shown in the figure above, the plot shows the training and test set accuracy on the yaxis against the setting of neighbors on the x-axis. Imagine if we only choose one neighbor, the predictions in the training set are perfect. However, when more neighbors are added, the training accuracy will decrease, which means that the model obtained by selecting only one neighbor is too complicated. The best practice is to choose around 9 neighbors. 

Output: 
Accuracy of K-NN classifier on training set: 0.79 

Accuracy of K-NN classifier on test set: 0.78 

Take user input to predict diabetes: 
In this section of code, we have uses voice system that tells to give input. Here the program will take the report of ‘Glucose’, ‘BloodPressure’, ‘SkinThickness’, ‘Insulin’, ‘BMI’, ‘DiabetesPedigreeFunction’, ‘Age’ as input. 
The output of the code will predict whether a person has diabetes or not.

Output: 
Analysis the user input the system will predict diabetes ‘yes’ or ’not, 

DECISION TREE: 
A decision tree is a decision support tool that uses a tree-like graph or model of decisions and their possible consequences, including chance event outcomes, resource costs, and utility. It is one way to display an algorithm that only contains conditional control statements. 
 
Accuracy Result:  
The accuracy on the training set is 100%, while the test set accuracy is much worse. This is an indicative that the tree is overfitting and not generalizing well to new data. Therefore, we need to apply prepruning to the tree. 

Accuracy on training set: 1.000 

Accuracy on test set: 0.714 

We set max_depth=3, limiting the depth of the tree decreases overfitting. This leads to a lower accuracy on the training set, but an improvement on the test set. 
 
Accuracy on training set: 0.773 

Accuracy on test set: 0.740 
