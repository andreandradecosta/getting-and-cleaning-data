# Code Book

## Raw Data
The script assumes the data is extracted into ```./data``` directory.

## Output
The results will be saved in ```./data/tidy_data.txt```. The format of this file is:
```
subject activity    measurement         mean
1       WALKING     tBodyAcc-mean()-X   0.27733076
```
 * subject - id of the subject
 * activity - name of the activity
 * measurement - variable of the raw data
 * mean - mean based on the subject and activity

## The Process Used
 * Read train and test data
 * Extract the variables names and activities labels
 * Combine the measurements with the subjects and activities
 * Extract only the mean() and std() variables
 * Group the data by subject and activity to calculate the mean
