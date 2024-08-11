# SUMMER-Tabular-Project
## *DATA*  
https://www.kaggle.com/competitions/playground-series-s3e22/data?select=train.csv  


BRIEF OVERVIEW- While reading about this dataset, I found that it is synthetic (created by using algorithms and simulations based on generative artificial intelligence technologies) which explains certain inconsistencies. The Predict Health Outcomes of Horses project is dedicated to a multi-class classification challenge. The target variable is the horse's outcome, which makes it a nominal dataset.  

Definition of the challenge: The challenge is defined by kaggle and its objective is to apply machine learning to predict the outcome of horses based on various info given about each horse. Machine learning will enable us to see accurately what features define their outcome and efficiently match up the initial data outcome . This data is tabular, also comma separated with 377.52KB. The dataset provides Information about different individuals. Information like age, rectal temp, pulse, respiratory rate, temp of extremities, etc  

Approach: The approach in this repository formulates the problem as classification task because about 60% is classification data , using Random Forest as the model. Random Forest is an ensemble method that builds multiple decision trees and combines their predictions. This generally leads to better accuracy compared to individual decision trees, as it reduces the likelihood of overfitting and increases generalizability. Random Forest provides a measure of feature importance, helping to identify which features are most influential in making predictions.  

## *Summary of Workdone*
RAW Data INFO
Type: Tabular, comma-separated, nominal.

Input: CSV file of features

output: smoker/non-smoker flag in 1st column.

Size: 377 KB, 1236 rows and 29 columns Instances (Train, Test, Validation Split)

Summary of performance: The metrics used to evaluate the model performance were F-1 score, recall, accuracy, ROC Curve and confusion matrix.

# *Relevent files and role in the package.*  

Data_exploration_chall -Loading the dataset and exploring the information about the dataset.

Data_visualization_chall -contains visualizations to better understand and interpret data.

Data_Preprocessing_chall -cleaning and preparing the dataset, staging it for machine learning model.

Machine_learning_chall -Creates the model and evaluating the perfomance.  

# *Preprocessing / Clean up*
I dropped 3 columns including lesion_3. This column failed the chi square test(hypothesis test used to determine if there is a significant association between two categorical variables).  

Engineering- I one-hot encoded categorical columns. Label encoded the target column.  

# *Training*
Describe the training: I used Random Forest because it's a robust and versatile ensemble learning method that combines multiple decision trees to improve accuracy and reduce the risk of overfitting. Random Forest works well with both classification and regression tasks, handles various data types, and is particularly effective in dealing with noisy or imbalanced datasets. I trained the model by first splitting the dataset into training and test sets, split into typical 80-20. Then, I used the RandomForestClassifier from scikit-learn, setting the number of trees (n_estimators) to 80. The model was trained on the training data to learn patterns, and its performance was evaluated on the test data, where I predicted the probabilities of the classes and used them to generate ROC curves for each class in a multiclass classification scenario. Any difficulties? How did you resolve them? There was no difficulties while training but having to divide into classes took me some time.


# * Visualizations*
![image](https://github.com/user-attachments/assets/b25aa411-7289-41b2-aa4d-88f4b8685057)  
![image](https://github.com/user-attachments/assets/6e65b89f-d48d-4995-84fc-a8cf78522986)


#* MACHINE LEARNING*  
![image](https://github.com/user-attachments/assets/601237a2-7898-4592-b867-4543106f2062)  
![image](https://github.com/user-attachments/assets/46650536-ed17-46f5-bf6c-0f37b7a06473)


![image](https://github.com/user-attachments/assets/7d18d7d9-3340-4f1a-9a24-62629485dc8c)




### *Software Setup*
Library: numpy, scikit learn, pandas, matplotlib,spicy stats.  



# *Citation*  
Walter Reade, Ashley Chow. (2023). Predict Health Outcomes of Horses. Kaggle. https://kaggle.com/competitions/playground-series-s3e22
