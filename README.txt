The run_analysis.R script is composed of five steps to finally produce the text file "Tidy.txt":
The code uses 2 R packages including data.table and dplyr

Step 1 is merges the 'training' and 'test' data to create 1 data set called completeDataSEt

a) reads the training data corresponding subject and activity label files and merges it.
b) reads the test data corresponding subject and activity label files and merges it.
c) merges the training and testing data sets into file called CompleteDataSet

Step 2 extracts the mean and standard deviation for each measurement in CompleteDataSEt. 

a) extract column indices that have either mean or standard deviation in them 
b) add "Activity" and "Subject" columns to the list 
c) create 'extractedData' with the selected columns in the 'requiredColumns' then look at dimensions of 'requiredColumns'

Step 3 Use descriptive activity names to name the activities in the data set. 

Step 4 label the data with descriptive variable names 

Step 5 creates a 2nd, independant tidy data set with the average of  each variable for each activity in each subject; using the data from step 4.
