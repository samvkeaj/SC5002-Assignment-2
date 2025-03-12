# SC5002-Assignment-2

README file explaining the project, dataset, and steps taken and insights

**Dataset:** The dataset originates from a diabetes research setting. In this dataset, there is data for many variables that have shown to be related to diabetes, such as the plasma glucose concentration at 2 hours in an oral glucose tolerance test, blood pressure, serum insulin at 2 hours, Body Mass Index, and Diabetes Pedigree Function scores. Given the multifaceted nature of diabetes, no single variable is a good predictor of diabetes. For instance, while diabates may traditionally be associated with a high BMI, many patients of Asian ethnicities actually have a "skinny fat" physique, appearing skinny overall but having fat deposits specifically at the liver. 

Additionally, mimicking the complexities of data collection from patients in real life, there exist certain measurements with no available data. This also presents an opportunity to utilise data cleaning and data imputation methods.

**Project:** Here, we attempt to use Linear Regression and Ridge Regression to predict patients' Diabetes Pedigree Function scores. If the prediction proves to be reliable, then the model can be used to predict Diabetes Pedigree Function scores based on patient history and existing medical records. Subsequently, higher scores can then be used to make a recommendation to patients for an precautionary check-up. 

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
