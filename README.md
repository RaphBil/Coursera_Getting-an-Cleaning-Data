Coursera_Getting-an-Cleaning-Data
=================================

This file describes how the run_analysis.R script works.

First of all, unzip the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip and rename it as "data".

Place the folder "data" and the run_analysis.R script in the current working directory.
Then, use source("run_analysis.R") command.
After that, two output files will be generated and placed in the current working directory: 

    merged_data.txt : contains a data frame called cleanedData with 10299*68 dimension.
    data_with_means.txt : contains a data frame called result with 180*68 dimension.

Finally, use data <- read.table("data_with_means.txt") command to read the file. 
Since we are required to get the average of each variable for each activity and each subject, and there are 6 activities in total and 30 subjects in total, we have 180 rows with all combinations for each of the 66 features.
