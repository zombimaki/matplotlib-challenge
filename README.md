# matplotlib-challenge

Matplotlib Homework - The Power of Plots

The Pymaceuticals jupyter notebook uses Matplotlib,Pandas,Numpy, and Scipy performs the following to make observations and insights on the tumor treatment of mice:

1. The program starts by loading the Mouse_metadata.csv file and the Study_results.csv file found in the Resources folder. 
2. Both sets of data are merged into one dataframe that will be used to stage the data prior to cleaning it up.
3. The number of unique mice in the staging df gets displayed to the screen.
4. The program identifies mice with duplicate time points and displays them to the screen.
5. The program lists all of the records associated with the duplicate mice to the screen.
5. A new dataframe is created that excludes the duplicate mice records. This dataframe (mouse_study_df) is be used for the rest of the analyses.
6. The program checks to see if the exclusion was successful by checking if there are duplicates. If there are duplicates it prints those messages to the screen. If there are no duplcates it prints that message to the screen.
7. The program then prints a new count of unique mice to the screen.
8. The program generates a summary statistics table of Tumor Volume (mm3) values using groupby and summary statistical methods to the screen.
9. The program generates a summary statistics table of Tumor Volume (mm3) values using a single line of code.
10. A Bar Chart is created for number of mice tested by Drug Regimens using Pandas.
11. A Bar Chart is created for number of mice tested by Drug Regimens using PyPlot.
12. A Pie Chart is created for number of mice by gender using Pandas.
13. A Pie Chart is created for number of mice by gender using PyPlot.
14. A group by df is created for max timepoint by mouse id, and then is merged with the mouse_study_df to create a new last timepoint df.
15. Program loops through a list of treatments for each row in the last timepoint df  the following is performed for each treatment sample:
a. The tumor volumes are appended to a list which is then converted to a series.<br />
b. Quartiles are identifed from the series.<br />
c. IQR is calcualted by subtracting the value of the first quartile from the value of the third quartile.<br />
d. One step variable is set to 1.5.<br />
e. Lower bound is calculated by subtracting the result of one step multiplied by iqr from the 1st quartile.<br />
f. Upper bound is calculated by adding the result of one step multiplied by iqr to the 3rd quartile.<br />
g. A for loop that does through the tumor series and prints the values that are outliers as well as the treatment they appear in.<br />
16. A boxplot of final tumor volume accross the regimens is displayed to the screen.
17. A line plot of tumor volume vs timepoint is generated for a mouse in the Capomulin treatment.
18. A scatter plot of avg tumor volume vs avg mouse weight for the Capomulin sample is generated.
19. The correlation coefficient and a linear regression model is created for avg mouse weight and avg tumor growth and a scatter chart is generated.




