Data source (valid as of 2015-22-02): https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
run_analysis.R does the following:

1. Merges the test and training data sets to create one dataset. 
2. Reads features.txt and extracts only the measurements on the mean and standard deviation for each measurement.
3. Reads activity_labels.txt and applies descriptive activity names for the activities in the set: 
(laying, sitting, standing, walking, walkingdownstairs, walkingupstairs)
4. Label data set with descriptive names. Then merge the data frame containing features with data frames containing activity labels and subject IDs. Save the result as merged_clean_data.txt. The names of the attributes are similar to the following: tbodyacc-mean-x,tbodyacc-mean-y,tbodyacc-mean-z,tbodyacc-std-x,tbodyacc-std-y,tbodyacc-std-z,tgravityacc-mean-x,tgravityacc-mean-y
5. Creates a tidy data set with the average of each measurement for each activity and each subject and save as data_set_with_the_averages.txt
