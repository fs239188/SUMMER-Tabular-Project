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

Size: 29.2 MB, 1236 rows and 29 columns Instances (Train, Test, Validation Split): how many data points? : 82248 individuals training, 27417 for testing, 27417 for validation

Summary of performance: The metrics used to evaluate the model performance were F-1 score, recall, accuracy, ROC Curve and confusion matrix.

# *Relevent files and role in the package.*  

Data_exploration_chall -Loading the dataset and exploring the information about the dataset.

Data_visualization_chall -contains visualizations to better understand and interpret data.

Data_Preprocessing_chall -cleaning and preparing the dataset, staging it for machine learning model.

Machine_learning_chall -Creates the model and evaluating the perfomance.  

#*Preprocessing / Clean up*
I dropped 3 columns including lesion_3. This column failed the chi square test

#* Visualizations*
![image](https://github.com/user-attachments/assets/b25aa411-7289-41b2-aa4d-88f4b8685057)



### *Software Setup*
Library: numpy, scikit learn, pandas, matplotlib,spicy stats.  



# *Citation*  
Walter Reade, Ashley Chow. (2023). Predict Health Outcomes of Horses. Kaggle. https://kaggle.com/competitions/playground-series-s3e22
