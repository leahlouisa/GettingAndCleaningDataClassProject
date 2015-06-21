# GettingAndCleaningDataClassProject

This project was about acquiring accelerometer and gyroscope data, cleaning it up, and performing some basic summarization of it.

The script I created to accomplish this begins by reading in the necessary data from the many files where it resides.  Wherever files contained columns full of character strings instead of numbers, I used used stringsAsFactors=FALSE to prevent those character strings from being interpreted as factors.  Additionally, I took advantage of the col.names field when reading in the x_Train and x_Test files in order to save myself the work of naming the many columns in those files later on.

Next, because each of the three types of data was split across training and test sets, I simply merged the training and test sets for each by rows, using rbind().  I then renamed the first column of the "y" data set to "activity", and the firsts column of the "subject" data set to "subject".

Then I combined all three data frames into a single frame by columns using a simple cbind.  Next I selected out only those columns that had "mean()" or "std()" within their name, while also retaining the "subject" and "activity" columns.

Because some of my column names had undesirable characters in them, I went through and removed those characters, and gave the activity column values that were descriptions of activities rather than numbers, for greater legibility.

Finally, I calculate the average of each mean() or std() field per subject and activity, and export my results to a file called averagesPerActivitySubject.txt.
