Submission by: Jophy Joseph        Aug 07, 2022

Week 5-8 Assign. Part-II  

Objective:- Build a ML model to predict the employee compensation. The application is built using Spark.

Steps done
1.) Google Colab was used. 
2.) pyspark and findspark installed
3.) Spark session created
4.) Google drive mounted and the given Employee_Compensation.csv was read 
5.) Data analysed and pre-processed (redundant columns,rows with negative salaries and missing values dropped)
6.) EDA done - bar plots with target column (Total Compensation) and Heatmap (for numerical features)
7.) StringIndexer, followed by OHE done for the categorical features and the indexed dataframe is fitted and transformed to build an encodedDF
8.) VectorAssembler created using the numerical features and the OHE vectors and used to transform the encodedDF to an assembledDF
9.) An udf used to convert the assembledDF to a densefeatureDF
10.)StandardScaler object is used to fit and transform the densefeatureDF to a stdscaledDF, which can be used for model building
11.) Data split into training and test (70:30)
12.) Linear Regression is used to fit the trainDF and create a lr_model
13.) The lr_model is used to tranform the testDF and get the predictions
14.) The lr_model is persisted using the save method
15.) It is loaded and the predictions run again


