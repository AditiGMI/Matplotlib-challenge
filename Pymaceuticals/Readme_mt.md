Overview:

1. We have been given 2 data sets "Study result & "Mouse metadata". We need to merge these 2 with left joint &  Run the provided package dependency and data imports, 
Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. 
2. The merged Dataframe has a duplicate mouse ID "g989" that need to be removed. for this we will use the !=(not equal to) with "g989" so we get all the cells with that mouse ID. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps. 
Display the updated number of unique mice IDs.

Generate Summary Statistics:

3. Create a DataFrame of summary statistics. We will 2 methods, first is the traditional way using .mean(), .median() & so on functions to create a Dataframe with these calculations. Summary statistics includes:
A row for each drug regimen. The regimen names is the index column. for this we will use the groupby function along with the agg function.
A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

Bar Charts and Pie Charts:

4. Generate two bar charts. Both charts should be identical and show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.
    Create the first bar chart with the Pandas DataFrame.plot() method.
    Create the second bar chart with Matplotlib's pyplot methods.
5. Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.
    Create the first pie chart with the Pandas DataFrame.plot() method.
    Create the second pie chart with Matplotlib's pyplot methods.

Quartiles, Find Outliers, and Create a Box Plot

6. Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. 
Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.
Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.
Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.
7. Determine outliers by using the upper and lower bounds, and then print the results.
8. Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.

Create a Line Plot and a Scatter Plot

9. Select a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for l509 mouse.
10. Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

Calculate Correlation and Regression

9. Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.
10. lot the linear regression model on top of the previous scatter plot.

Final Analysis:

1. The sex ratio for both male & female mouse is the almost the same.
2. Capomulin & Ramicane drug work well compared to other 8 drugs 
3. Only Infubinol has an outlier value among the four drugs : Capomulin, Ramicane, Infubinol, and Ceftamin
4. Tumor Volume decrease over timepoints considerably with the use of Capomulin drug
5. In the summary scatter plot for the drug Capomulin there is a strong positive correlation between the Weight & Tumor volume of the mouse, which means: the y values tend to increase as the x values increases, in this case as the weight incraeses the tumor volume also increases.

