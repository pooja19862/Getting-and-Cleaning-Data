Getting and Cleaning Data : Project Assignment


Run_analysis.R : My R code that does the following things:
Merges the training and the test sets to create one data set and assign column names. Following files were merged:
features.txt
activity_labels.txt
subject_train.txt
x_train.txt
y_train.txt
subject_test.txt
x_test.txt
y_test.txt
Extracts only the measurements on the mean and standard deviation for each measurement.
Used grepl command to filter column names containg "mean", "std" and "Id"
Uses descriptive activity names to name the activities in the data set
Merge the finalData set with the acitivityType table to include descriptive activity names
Appropriately labels the data set with descriptive variable names.
Cleaned the variable names and made it more descriptive using gsub command
From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
Used dplyr package to group_by rows based on subjectID and activityID and used summarise_each command to calculate mean on other columns


