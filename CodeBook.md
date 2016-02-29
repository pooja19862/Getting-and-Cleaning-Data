**### Getting and Cleaning Data : Project Assignment**

This file gives description of Run_analysis.R code

My R code that does the following things:
1. Merges the training and the test sets to create one data set and assign column names.
Following files were merged:
- features.txt
- activity_labels.txt
- subject_train.txt
- x_train.txt
- y_train.txt
- subject_test.txt
- x_test.txt
- y_test.txt

2. Extracts only the measurements on the mean and standard deviation for each measurement
Used grepl command to filter column names containg "mean", "std" and "Id"

3. Uses descriptive activity names to name the activities in the data set
Merge the finalData set with the acitivityType table to include descriptive activity names

4. Appropriately labels the data set with descriptive variable names.
Cleaned the variable names and made it more descriptive using _gsub_ command

3. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
Used _dplyr_ package to _groupby_ rows based on subjectID and activityID and used _summariseeach_ command to calculate mean on other columns
