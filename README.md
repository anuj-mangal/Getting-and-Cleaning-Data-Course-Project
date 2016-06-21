# Getting-and-Cleaning-Data-Course-Project
The repository has  been created to share the final artifacts created as part of this project work

##Script Description

1. There is a single script as part of this project, named 'run_analysis.R'.

2. The script first imports the reshape2 package which brings dcast() and melt() functions to the current working environment.

3. In the second step, it resets the environment and removes any previously created variables.

4. The data is read from all the input files into data frames.

5. In the following steps, I am merging training and testing datasets for feature values, activities and subjects.

6. The merge of the datasets is followed by the assignment of header or variable names in the respective datasets.

7. Next, via the use of grep, I am extracting the measures which are related to the calculation of means and standard deviation of variables.

8. Now I am merging the data of activities and subjects with the measurements. post this step I am using merge function to derive the activity name from the      activity_label data frame.

9. Next step is to rename the variables in the complete_data data frame with more descriptive ones.

10. As part of the penultimate step, I am melting the data frame and recasting it against activity_id, activity_name and subject_id to calculate the means of the variables.

11. The last step is to call the write.table function to write the final data frame i.e. final_data to a text file named "tidy_data.txt".

 
