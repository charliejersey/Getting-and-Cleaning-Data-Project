# Codebook for Getting and Cleaning Data Project

# Source Data

The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. The data is A full description is available at the site where the data was obtained:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Here is the data for the project:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

# R file(code)

File with R code "run_analysis.R" will perform steps 1-5 outlines in the readme.md link in repository

# Code Variables

x_Train, y_Train, subject_Train, x_Test, y_Test, subject_Test are the downloaded files associated from the zip link above.  Each variable name has the same name as the file associated in the download.

merge_Train merges the data from y_Train, subject_Train, x_Train by the command cbind

merge_test merges the data from y_Test, subject_Test, x_Test by the command cbind

merge_Data merges the data from merge_Train and merge_test into one big data set by the rbind command

subject_Features is used to name the columns of the merge_Train dataset

subject_Activity is used to is a similar way applied to column names

MeanAndStd is used to store all the columns and values below that have a mean or std

Finally tidydataset2 is used to create the second tidy data set with the average of each variable on activity and subject

# .tidydataset2 Columns

tBodyAccMeanX,
tBodyAccMeanY,
tBodyAccMeanZ,
tBodyAccStdX,
tBodyAccStdY,
tBodyAccStdZ,
tGravityAccMeanX,
tGravityAccMeanY,
tGravityAccMeanZ,
tGravityAccStdX,
tGravityAccStdY,
tGravityAccStdZ,
tBodyAccJerkMeanX,
tBodyAccJerkMeanY,
tBodyAccJerkMeanZ,
tBodyAccJerkStdX,
tBodyAccJerkStdY,
tBodyAccJerkStdZ,
tBodyGyroMeanX,
tBodyGyroMeanY,
tBodyGyroMeanZ,
tBodyGyroStdX,
tBodyGyroStdY,
tBodyGyroStdZ,
tBodyGyroJerkMeanX,
tBodyGyroJerkMeanY,
tBodyGyroJerkMeanZ,
tBodyGyroJerkStdX,
tBodyGyroJerkStdY,
tBodyGyroJerkStdZ,
tBodyAccMagMean,
tBodyAccMagStd,
tGravityAccMagMean,
tGravityAccMagStd,
tBodyAccJerkMagMean,
tBodyAccJerkMagStd,
tBodyGyroMagMean,
tBodyGyroMagStd,
tBodyGyroJerkMagMean,
tBodyGyroJerkMagStd,
fBodyAccMeanX,
fBodyAccMeanY,
fBodyAccMeanZ,
fBodyAccStdX,
fBodyAccStdY,
fBodyAccStdZ,
fBodyAccMeanFreqX,
fBodyAccMeanFreqY,
fBodyAccMeanFreqZ,
fBodyAccJerkMeanX,
fBodyAccJerkMeanY,
fBodyAccJerkMeanZ,
fBodyAccJerkStdX,
fBodyAccJerkStdY,
fBodyAccJerkStdZ,
fBodyAccJerkMeanFreqX,
fBodyAccJerkMeanFreqY,
fBodyAccJerkMeanFreqZ,
fBodyGyroMeanX,
fBodyGyroMeanY,
fBodyGyroMeanZ,
fBodyGyroStdX,
fBodyGyroStdY,
fBodyGyroStdZ,
fBodyGyroMeanFreqX,
fBodyGyroMeanFreqY,
fBodyGyroMeanFreqZ,
fBodyAccMagMean,
fBodyAccMagStd,
fBodyAccMagMeanFreq,
fBodyBodyAccJerkMagMean,
fBodyBodyAccJerkMagStd,
fBodyBodyAccJerkMagMeanFreq,
fBodyBodyGyroMagMean,
fBodyBodyGyroMagStd,
fBodyBodyGyroMagMeanFreq,
fBodyBodyGyroJerkMagMean,
fBodyBodyGyroJerkMagStd,
fBodyBodyGyroJerkMagMeanFreq,

# Activities 

WALKING = 1 Walking with the Samsung Device,
WALKING_UPSTAIRS = 2 Walking Upstairs with the Samsung Device,
WALKING_DOWNSTAIRS = 3 Walking Downstairs with the Samsung Device,
SITTING = 4 Sitting with the Samsung Device,
STANDING = 5 Standing with the Samsung Device,
LAYING = 6 Laying with the Samsung Device,
