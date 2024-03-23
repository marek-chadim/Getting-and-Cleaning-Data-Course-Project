# Getting-and-Cleaning-Data-Course-Project

The purpose of this project is to demonstrate  ability to collect, work with, and clean a data set. 

Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. 
The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. 
A full description is available at the site where the data was obtained:

- http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

 
Here are the data for the project:

 - https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

  
 R script called run_analysis.R  does the following

  -  Merges the training and the test sets to create one data set.

  -  Extracts only the measurements on the mean and standard deviation for each measurement. 

   - Uses descriptive activity names to name the activities in the data set

  -  Appropriately labels the data set with descriptive variable names. 

   - From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.



```{r }
tidyData <- read.csv("tidyData.txt")
as_tibble(tidyData)

# A tibble: 180 × 68
   SubjectNum Activity           `tBodyAcc-mean-X` `tBodyAcc-mean-Y` `tBodyAcc-mean-Z` `tBodyAcc-std-X` `tBodyAcc-std-Y` `tBodyAcc-std-Z` `tGravityAcc-mean-X`
   <fct>      <fct>                          <dbl>             <dbl>             <dbl>            <dbl>            <dbl>            <dbl>                <dbl>
 1 1          WALKING                        0.277          -0.0174            -0.111           -0.284           0.114            -0.260                 0.935
 2 1          WALKING_UPSTAIRS               0.255          -0.0240            -0.0973          -0.355          -0.00232          -0.0195                0.893
 3 1          WALKING_DOWNSTAIRS             0.289          -0.00992           -0.108            0.0300         -0.0319           -0.230                 0.932
 4 1          SITTING                        0.261          -0.00131           -0.105           -0.977          -0.923            -0.940                 0.832
 5 1          STANDING                       0.279          -0.0161            -0.111           -0.996          -0.973            -0.980                 0.943
 6 1          LAYING                         0.222          -0.0405            -0.113           -0.928          -0.837            -0.826                -0.249
 7 2          WALKING                        0.276          -0.0186            -0.106           -0.424          -0.0781           -0.425                 0.913
 8 2          WALKING_UPSTAIRS               0.247          -0.0214            -0.153           -0.304           0.108            -0.112                 0.791
 9 2          WALKING_DOWNSTAIRS             0.278          -0.0227            -0.117            0.0464          0.263            -0.103                 0.862
10 2          SITTING                        0.277          -0.0157            -0.109           -0.987          -0.951            -0.960                 0.940
# ℹ 170 more rows
# ℹ 59 more variables
```

