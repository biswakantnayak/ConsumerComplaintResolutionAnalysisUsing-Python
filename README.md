# Consumer Complaint Resolution Analysis Using Python 

## Objective:
**Used Python libraries such as Pandas for data operations, Seaborn and Matplotlib for data visualization and 
EDA tasks, Sklearn for model building and performance visualization, and based on the best model, 
make a prediction for the test file and save the output.**

## Tools & Libraries
- **Tools:** Python & Jupyter notebook
- **Libraries:** pandas, numpy, seaborn, matplotlib, sklearn.model_selection, 
                 sklearn.preprocessing, sklearn.decomposition, sklearn.linear_model, 
                 sklearn.tree, sklearn.ensemble, sklearn.neighbors, sklearn.metrics, 
                 xgboost & warnings 

## Problem Statement
1. Read the Data from the Given excel file.
2. Check the data type for both data (test file and train file)
3. Do missing value analysis and drop columns where more than 25% of data are missing
4. Extracting Day, Month, and Year from Date Received Column and create new fields for a month, year, and day
5. Calculate the Number of Days the Complaint was with the Company and create a new field as “Days held”
6. Drop "Date Received","Date Sent to Company","ZIP Code", "Complaint ID" fields
7. Imputing Null value in “State” by Mode
8. with the help of the days we calculated above, create a new field 'Week_Received' where we calculate the week based on the day of receiving.
9. store data of disputed people into the “disputed_cons” variable for future tasks
10. Plot bar graph of the total no of disputes of consumers with the help of seaborn
11. Plot bar graph of the total no of disputes products-wise with the help of seaborn
12. Plot bar graph of the total no of disputes with Top Issues by Highest Disputes, with the help of seaborn
13. Plot bar graph of the total no of disputes by State with Maximum Disputes
14. Plot bar graph of the total no of disputes Submitted Via different source
15. Plot bar graph of the total no of disputes where the Company's Response to the Complaints
16. Plot bar graph of the total no of disputes where the Company's Response Leads to Disputes
17. Plot bar graph of the total no of disputes. Whether there are Disputes Instead of Timely Response
18. Plot bar graph of the total no of disputes over Year Wise Complaints
19. Plot bar graph of the total no of disputes over Year Wise Disputes
20. Plot bar graph of Top Companies with Highest Complaints
21. Converte all negative days held to zero (it is the time taken by the authority that can't be negative)
22. Drop Unnecessary Columns for the Model Building
  like:'Company', 'State', 'Year_Received', 'Days_held'
23. Change Consumer Disputed Column to 0 and 1(yes to 1, and no to 0)
24. Create Dummy Variables for categorical features and concat with the original data framelike: 'Product,’ 'Submitted via,’ 'Company response to consumer,’ 'Timely response?'
25. Scaling the Data Sets (note: discard dependent variable before doing standardization)and Make feature Selection with the help of PCA up to 80% of the information.
26. Splitting the Data Sets Into X and Y by the dependent and independent variables (data selected by PCA)
27. Build given models and measure their test and validation accuracy:
    - LogisticRegression
    - DecisionTreeClassifier
    - RandomForestClassifier
    - AdaBoostClassifier
    - GradientBoostingClassifier
    - KNeighborsClassifier
    - XGBClassifier
28. Whoever gives the most accurate result uses it and predicts the outcome for the test file and fills its dispute column so the business team can take some action accordingly.

## Process:
1. **Exploratory Data Analysis**
2. **Feature Engineering**  
3. **Visualization**  
4. **Modeling building & Evaluation**   
5. **Prediction on Test File**

## Key Features
- Extracted features like:
  - `Day`
  - `Month`
  - `Year` 
  - `Days Held`
  - `Week Received`
  
- Visualized disputes by:
  - Numbers of disputes
  - Product
  - State
  - Via different source
  - Company's Response
  - Top Issues
  - Timely Response
  - Year Wise Disputes 
  - Highest Complaints 
  
- Modeled binary classification using 7 ML algorithms
- Selected best model based on accuracy for final test prediction

## Outcome:
**The final model helps predict whether a `customer will dispute` a complaint based on the information available at 
the time of submission. This can be used by the business team to prioritize or investigate complaints more efficiently.**
