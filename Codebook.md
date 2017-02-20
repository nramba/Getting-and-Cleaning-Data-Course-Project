
**Script attached : run_analysis.R**

# Approach : 

1.Initially, the similar data (Same number of columns and data) is merged using rbind().

2.The only columns having mean and SD measures are extracted from the combined dataset and are correctly named as from features.txt

3.The activity data is present in values 1:6, which we take from the file activity_labels.txt and are appended to the dataset.

4.Finally, we generate a dataset(Write function) with all the average measures for each subject and activity type into a file named averages_data.txt.

# Explaination of variables :

1. Variables : x_train, y_train, x_test, y_test, subject_train and subject_test are the data from the downloaded files, x_data, y_data and subject_data contain the merged datasets.

2.Features contains the revised names for the x_data dataset, which are applied to the column names stored in mean & _std_features, a numeric vector used to extract the desired data.Likewise, the same is performed on the activities variable

3.all_data is a merged data set of x_data, y_data and subject_data.

4.Then, average_data contains the averages which will be later stored in a .txt file.