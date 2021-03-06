---
title: "Getting and Cleaning Data: Class Project Codebook"
output: html_document
---

**Column Name: "activity"**

Describes which of the six activities applies to this row.

**Column Name: "subject"**

The number of the test subject.

**All Other Columns:**

These columns include the following:

"tBodyAccmeanX", "tBodyAccmeanY", 
"tBodyAccmeanZ", 
"tGravityAccmeanX", 
"tGravityAccmeanY", 
"tGravityAccmeanZ", 
"tBodyAccJerkmeanX", 
"tBodyAccJerkmeanY", 
"tBodyAccJerkmeanZ", 
"tBodyGyromeanX", 
"tBodyGyromeanY", 
"tBodyGyromeanZ", 
"tBodyGyroJerkmeanX", 
"tBodyGyroJerkmeanY", 
"tBodyGyroJerkmeanZ", 
"tBodyAccMagmean", 
"tGravityAcMagmean", 
"tBodyAccJerkMagmean", 
"tBodyGyroMagmean", 
"tBodyGyroJerkMagmean", 
"fBodyAccmeanX", 
"fBodyAccmeanY", 
"fBodyAccmeanZ", 
"fBodyAccJerkmeanX", 
"fBodyAccJerkmeanY", 
"fBodyAccJerkmeanZ", 
"fBodyGyromeanX", 
"fBodyGyromeanY", 
"fBodyGyromeanZ", 
"fBodyAccMagmean", 
"fBodyBodyAccJerkMagmean", 
"fBodyBodyGyroMagmean", 
"fBodyBodyGyroJerkMagmean", 
"tBodyAccstdX", 
"tBodyAccstdY", 
"tBodyAccstdZ", 
"tGravityAccstdX", 
"tGravityAccstdY", 
"tGravityAccstdZ", 
"tBodyAccJerkstdX", 
"tBodyAccJerkstdY", 
"tBodyAccJerkstdZ", 
"tBodyGyrostdX", 
"tBodyGyrostdY", 
"tBodyGyrostdZ", 
"tBodyGyroJerkstdX", 
"tBodyGyroJerkstdY", 
"tBodyGyroJerkstdZ", 
"tBodyAccMagstd", 
"tGravityAccMagstd", 
"tBodyAccJerkMagstd", 
"tBodyGyroMagstd", 
"tBodyGyroJerkMagstd", 
"fBodyAccstdX", 
"fBodyAccstdY", 
"fBodyAccstdZ", 
"fBodyAccJerkstdX", 
"fBodyAccJerkstdY", 
"fBodyAccJerkstdZ", 
"fBodyGyrostdX", 
"fBodyGyrostdY", 
"fBodyGyrostdZ", 
"fBodyAccMagstd", 
"fBodyBodyAccJerkMagstd", 
"fBodyBodyGyroMagstd", 
"fBodyBodyGyroJerkMagstd" 

For all of the variables listed above, the average value of the variable for the given activity and test subject was calculated using the mean() function in R across a body of data gathered by Jorge L. Reyes-Ortiz, Alessandro Ghio, Luca Oneto, and Davide Anguita.  Because it is a calculated mean, the entries each retain the original units of the measurements they are averaging, whether from the time or frequency domain.

The following quote from the paper "Human Activity Recognition on Smartphones using a Multiclass Hardware-Friendly Support Vector Machine" describes the original measurements whose averages are shown here:
<pre>
The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 

These signals were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

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

The set of variables that were estimated from these signals are: 

mean(): Mean value
std(): Standard deviation
</pre>


