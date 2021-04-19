Description of Analysis
This analysis script run_analysis.R summarizes the mean and standard deviation data from the UCI HAR dataset. The original dataset is avaialble here: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

Run Analysis
Here are the data for the analysis:

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

Checks for required packagges and installs if necessary.
Downloads the data archive from the above URL.
Reads the files from the UCI HAR dataset, including activity names, subject identifier, measurement variables and measured data.
Merges the training and the test sets to create one data set.
Combines the activities and measurement data.
Adds the subject identity as a column to the measurement data.
Extracts only the measurements on the mean and standard deviation for each measurement.
Substitute descriptive activity names to name the activities in the data set.
Applies descriptive labels to the measurement variables the data set.
From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
To run this analysis, copy the script run_analysis.R to your working directory and source the script. In addition to base r, it requires the dplyr, stringr and reshape2 packages. The script will check whether the packages are installed and install them if necessary.

This script will output a file named meanDataTidy.csv.
