## Coursera-Getting and Cleaning Data-Course Project
This README file summarizes the instructions for Getting and Cleaning Data Course Project and explains how the R script run_analysis.R works to perform the tasks in the project.
## Project instructions:
Basically project asks to create R script run_analysis.R to perform following steps.
1.	Merges the training and the test sets to create one data set.
2.	Extracts only the measurements on the mean and standard deviation for each measurement. 
3.	Uses descriptive activity names to name the activities in the data set
4.	Appropriately labels the data set with descriptive variable names. 
5.	From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
## Explanation of R script run_analysis.R
The R script run_analysis.R has five different parts according to what is being asked in the project work.
Part-1 of the code reads all the required files and forms the complete data set; function rbind() is used to form data set.
Part-2 of the script extracts measurements on the mean and standard deviation for each measurement. Note that only measurements with mean() and std are extracted; function grep() is used to extract these measurements.
Part-3 labels the activity names for respective activities in the data set.
Part-4 labels the data set with descriptive variable names, function gsub() is used to perform this task. Below are the modifications done in the given variable names to make variable names more clear.
Acc to Accelerator; Gyro to Gyroscope; Mag to Magnitude;  t to TimeDomain; f to FrequencyDomain; std to StandardDeviation, etc
Part-5 creates tidy data from data in step-4 with the average of each variable for each activity and each subject; functions melt() and dcast are used to perform this task.

## Running the script:
Please make sure to set the working directory at the start of the script before running the script.

## Additional information:
Please refer the CodeBook.md for more information about the variables, data, etc.

