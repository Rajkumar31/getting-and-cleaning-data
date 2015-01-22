# getting-and-cleaning-data

## Methodology
Create one R script called run_analysis.R that does the following:
 1. Merges the training and the test sets to create one data set.
 2. Extracts only the measurements on the mean and standard deviation for each measurement.
 3. Uses descriptive activity names to name the activities in the data set
 4. Appropriately labels the data set with descriptive activity names.
 5. Creates a second, independent tidy data set with the average of each variable for each activity and each subject.

## Variables

activity_labels - Loads the activity labels dataset into it

features - Contains all the features of the dataset

extract_features - Extract only the measurements on the mean and standard deviation for each measurement

x-test, y-test - Load and process Xtest & ytest data

test_data - Data that is binded and ready to be used as a test set

x-train, y-train - Load and process Xtrain & ytrain data

train_data - Data that is binded and ready to be used as a test 

data - Row binded data of both test and train data set

## Functions

## Melt
The melt function takes data in wide format and stacks a set of columns into a single column of data. To make use of the function we need to specify a data frame, the id variables (which will be left at their settings) and the measured variables (columns of data) to be stacked. The default assumption on measured variables is that it is all columns that are not specified as id variables.

## Dcast
dcast uses a formula to describe the shape of the data. The arguments on the left refer to the ID variables and the arguments on the right refer to the measured variables. 
