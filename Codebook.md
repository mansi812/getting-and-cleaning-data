 data was downloaded in the working directory using  download.file command 
Zip file was unzipped using unzip command
Training and test data sets were separately merged using rbind command.
The mean and Standard deviations measurements were extracted using the grep command.
Grep command matches the arguments containing only mean and std in their names.
The indices of feature file containing mean and std in their names were found using 
mean.sd <- grep("-mean\\(\\)|-std\\(\\)", features[, 2])  command
gsub command is used to replace all the undesrcores with “”
Using the indices found earlier (mean.sd) ,names were given to all the activities in X dataset
Tidydata set was formed using the cbind column
Lapply column has been used to measure mean and SD across Subject ID and Activity


Following are the activity measurements for the data

tBodyAcc-XYZ
tGravityAcc-XYZ
tBodyAccJerk-XYZ
tBodyGyro-XYZ
tBodyGyroJerk-XYZ
tBodyAccMag
tGravityAccMag
tBodyAccJerkMag
tBodyGyroMag
tBodyGyroJerkMag
fBodyAcc-XYZ
fBodyAccJerk-XYZ
fBodyGyro-XYZ
fBodyAccMag
fBodyAccJerkMag
fBodyGyroMag
fBodyGyroJerkMag

The data is grouped by the follwong activities:
 (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING
 
 
