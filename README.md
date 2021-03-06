## Introduction

This assignment contains the below 4 files

1. CodeBook.md - Descripts the original data sets, transformation process and the new data set that was derived.

2. run_analysis.R - contains the R code to read the original data sets, transform the sets and write a cleaned and processed data set in file "tidy_data.txt"

3. README.md - This file which describes all the files uploaded as part of this assignment

4. tidy_data.txt - This is the output generated by run_analysis.R file that has the tidy data set as explained by CodeBook.md. The same has also been uploaded as text file as part of the assignment submission.


#### Brief overview of the assignment activities
This assignment/script uses data from: 

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

Unzips the file in current working directory retaining the directory structure

The details of the original data sets used and the transformation steps performed by the script is explained in CodeBook.md

The script reads the respective training data sets and test data sets and horizontally merges these two data sets. 

The script then performs the required data transformation to clean and process the data.

The tidy data is then stored in the current working directory "tidy_data.txt"

To load the data in R you can use the below command ()


    file_path <- "tidy_data.txt"
    data <- read.table(file_path, header = TRUE)
    View(data)
    
This code is based on the inputs from discussion thread - https://class.coursera.org/getdata-008/forum/thread?thread_id=24

In order to get the variables names for the CodeBook.md, used the below command in R

    writeLines(names(tidyData), "var_names.txt")
    
and copied the data from var_names.txt into the CodeBook.md file.

Thank you.