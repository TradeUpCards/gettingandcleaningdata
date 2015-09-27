# gettingandcleaningdata
# Coursera Getting And Cleaning Data Course

## Course Project
### Data
The data for this project can be found here:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

## run_analysis.R
### Process
1. Set the wd

	Set the wd to the same folder containing the run_analysis.R script.

1. Read in the training and test data
	- Reads the train data in
	- Binds the train data together (data frame: t)
	- Reads the test data in
	- Binds the test data together (data frame: v)
	- Binds the train and test data together (data frame: alldata)
	
1. Names the columns using the features.txt file
2. Subsets the alldata data frame to only mean and sd measurements (data frame: allmeansd)
3. Changes the Activity column to a factor and applies the descriptive names to Activity
4. Summarizes the data by aggregating the measurements by Subject + Activity groups (data frame: df)
5. Writes out the data frame df
6. The last line of code is how to read back in the output file into R
