# SC5002-Assignment-2

README file explaining the project, dataset, and steps taken and insights

**Dataset:** The dataset originates from a diabetes research setting. In this dataset, there is female patient data for many variables that have shown to be related to diabetes, such as the plasma glucose concentration at 2 hours in an oral glucose tolerance test, blood pressure, serum insulin at 2 hours, Body Mass Index, and Diabetes Pedigree Function scores. Given the multifaceted nature of diabetes, no single variable is a good predictor of diabetes. 

There are 9 features in the dataset which provide valuable information related to risk factors and indicators of diabetes:
1) Pregnancies: Number of pregnancies; gestational diabetes increases the risk of type 2 diabetes later in life.
2) Glucose: Blood sugar levels; elevated glucose is a key sign of type 2 diabetes and insulin resistance.
3) BloodPressure: High blood pressure is a comorbidity with diabetes, often worsened by insulin resistance.
4) SkinThickness: Indicator of subcutaneous fat; higher thickness may suggest insulin resistance and higher diabetes risk.
5) Insulin: Measures insulin levels; insulin resistance leads to higher levels as the body compensates.
6) BMI: Body Mass Index; obesity is strongly linked to type 2 diabetes and insulin resistance.
7) DiabetesPedigreeFunction: Genetic predisposition to diabetes based on family history; higher values indicate a greater risk.
8) Age: Risk of type 2 diabetes increases with age, especially after 45, due to insulin resistance and lifestyle factors.
9) Outcome: Target variable (1 = diabetic, 0 = non-diabetic); used to assess model’s predictive ability for diabetes risk.

Additionally, mimicking the complexities of data collection from patients in real life, there exist certain measurements with no available data. This also presents an opportunity to utilise data cleaning and data imputation methods.

**Project:** Here, we attempt to use Linear Regression and Ridge Regression to see if an accurate prediction can be made for BMI, specifically in women. If the prediction proves to be reliable, then it means that there exists a feasible relationship between BMI and the variables. Hence, BMI can still be used as a simple and quick indicator of health in patients, particularly in the input features, such as the Diabetes Pedigree Function scores, patient history and existing medical records. Indeed, if a patient experiences a sudden, drastic increase in her BMI, then it could be an indication in the change of health in one, or many of the input features. Particularly, BMI, as a quick and visible metric, remains most accessible to many poorer or less-developed communities. 

**Steps taken:**

Briefly, the steps taken are as follows

1. Vetting of a few different datasets - some datasets were too huge, or had questionable integrity
2. Superficial check for missing values, by looking for empty strings or null values
3. Deeper check of dataset for data integrity issues
4. Data cleaning - removing certain rows, and imputing missing data for others
5. Creating function for model training, with built-in encoding of categorical values and scaling of numerical values
6. Specifying input features and continous output
7. Perform train-test split, and calculate performance metrics (MSE and R<sub>2</sub>)
8. Conduct k-fold cross validation, and calculate performance metrics
9. Analysis and discussion of results

**Insights:**
BMI could be a feasible predictor of poor health inputs in diabetic patients, especially in the case where devices and techniques needed for more in-depth measurements are not available.

The results also show that Linear Regression alone performs well enough, with no notable gains from regularization. This suggests that Linear Regression may be a practical choice for clinical settings where simplicity and interpretability are important.

**Link to slides:** https://www.canva.com/design/DAGhP8nwpV0/xQ_HGqgKAtksZld-Vcv0nQ/edit

**Individual Contributions** (Clearly highlight the contributions of each team member in both the GitHub repository and the video)
1. Both Bryant and Yuen In were involved in selecting datasets, with a total of 2 datasets examined by Bryant and 1 dataset examined by Yuen In before the final dataset was selected for use. 
2. Bryant and Jing Yun added text cells with explanations, such that the notebook had a smooth logical flow.
3. Bryant was responsible for handling missing values in the dataset.
4. Yuen In was responsible for encoding categorical variables using One-Hot Encoding, and scaling numerical features using Min-Max Scaling.
5. Bryant was responsible for splitting the data into test and training data sets.
6. Yuen In wrote the bulk of the code for Linear Regression, Ridge Regression, and k-fold cross validation, with adaptation of the code to the datasets done by Bryant.
7. Jing Yun was responsible for comparing the models using Mean Squared Error (MSE) and R² score, and analysing cases where Linear Regression overfits and where Ridge Regression helps
prevent overfitting.
8. Jing Yun was responsible for interpreting the effect of different alpha values on the MSE and R^2 scores of the Ridge Regression Model, as well as discussing practical applications where each model would be more suitable.
9. Bryant was responsible for the overall project management, including the GitHub repository.
10. Jing Yun and Bryant put together the slides.
