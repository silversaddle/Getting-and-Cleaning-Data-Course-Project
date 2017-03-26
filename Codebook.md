# Code Book

This document describes the code inside `run_analysis.R`.

The code is splitted (by comments) in some sections:

* Download the Data
* Unzip DataSet to /data directory
* Load Packages
* Set file Path
* Create DataTables
* Manipulating data
* Writing final data to CSV


### Download the Data

Downloads the given url to the given destiny file. It also creates `data` dir if it doesn't exist.

#### Unzip DataSet to /data directory

Unzips zip file 

###Load Packages
Loads dplyr, data.table, and tidyr packages

###Set file Path
Sets file path


### Create DataTables

Read dataset files from UCI HAR to given name and prefix. Know names are "train" and "test". Known prefixes are "X", "y" and "subject".

Examples:

* `UCI HAR Dataset/train/X_train.txt`
* `UCI HAR Dataset/train/y_train.txt`
* `UCI HAR Dataset/train/subject_train.txt`


Loads data, labels and subjects from UCI HAR dataset to a `data.frame`.
The returned `data.frame` contains a column `Activity` with labels integer codes, a column `Subject` with subjects integer codes and all other columns from data.


## Manipulating data

*Merges the training and the test sets to create one data set and rename variables "subject" and "activityNum"

## Writing final data to CSV

Writes the TidyData.csv.
