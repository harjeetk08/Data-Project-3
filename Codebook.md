Code Book for Project 3 

Overview

Source of the original data:

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
Full Description at the site where the data was obtained:

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
Process

The script run_analysis.R performs the following process to clean up the data and create tiny data sets:

Merges the training and the test sets to create one data set.

Extracts only the measurements on the mean and standard deviation for each measurement.

Uses descriptive activity names to name the activities in the data set

Appropriately labels the data set with descriptive variable names.

From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

Variables

Values of Varible Activity consist of data from “Y_train.txt” and “Y_test.txt”

values of Varible Subject consist of data from “subject_train.txt” and subject_test.txt"

Values of Varibles Features consist of data from “X_train.txt” and “X_test.txt”

Names of Varibles Features come from “features.txt”

levels of Varible Activity come from “activity_labels.txt”

So we will use Activity, Subject and Features as part of descriptive variable names for data in data frame.

prefix t is replaced by time
Acc is replaced by Accelerometer
Gyro is replaced by Gyroscope
prefix f is replaced by frequency
Mag is replaced by Magnitude
BodyBody is replaced by Body

names(Data)
##  [1] "timeBodyAccelerometer-mean()-X"                
##  [2] "timeBodyAccelerometer-mean()-Y"                
##  [3] "timeBodyAccelerometer-mean()-Z"                
##  [4] "timeBodyAccelerometer-std()-X"                 
##  [5] "timeBodyAccelerometer-std()-Y"                 
##  [6] "timeBodyAccelerometer-std()-Z"                 
##  [7] "timeGravityAccelerometer-mean()-X"             
##  [8] "timeGravityAccelerometer-mean()-Y"             
##  [9] "timeGravityAccelerometer-mean()-Z"             
## [10] "timeGravityAccelerometer-std()-X"    
.
.
.



