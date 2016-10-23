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


Codebook:


Description of abbreviations of measurements

leading t or f is based on time or frequency measurements.
Body = related to body movement.
Gravity = acceleration of gravity
Acc = accelerometer measurement
Gyro = gyroscopic measurements
Jerk = sudden movement acceleration
Mag = magnitude of movement
mean and SD are calculated for each subject for each activity for each mean and SD measurements.
The units given are g’s for the accelerometer and rad/sec for the gyro and g/sec and rad/sec/sec for the corresponding jerks.

These signals were used to estimate variables of the feature vector for each pattern:
‘-XYZ’ is used to denote 3-axial signals in the X, Y and Z directions. They total 33 measurements including the 3 dimensions - the X,Y, and Z axes.

tBodyAcc-XYZ
tGravityAcc-XYZ
tBodyAccJerk-XYZ
tBodyGyro-XYZ
tBodyGyroJerk-XYZ
tBodyAccMag
tGravityAccMag
tBodyAccJerkMag
tBodyGyroMag
tBodyGyroJerkMag
fBodyAcc-XYZ
fBodyAccJerk-XYZ
fBodyGyro-XYZ
fBodyAccMag
fBodyAccJerkMag
fBodyGyroMag
fBodyGyroJerkMag
The set of variables that were estimated from these signals are:

mean(): Mean value
std(): Standard deviation

end