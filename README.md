# SA-Crime-Data
This project involves the merging of various data files, data correction, data visualization, data analysis using linear regression and choropleth mapping. Note: Data files are too large to upload.

In the accompanying jupyter notebook, Crime Statistics for the whole of South Africa (broken down by crime type, year, province and Police Station is imported into the notebook. This data is merged with a csv file of Police Station coordinates (based on Police Station name). 
Errors related to naming of the Crime Type (eg: use of both CONTACT CRIMES and CONTACT CRIME in the data file) are then corrected. 
The resultant data file is then saved as a csv for further analysis in Tableau.

Within the jupyter notebook some exploratory data analysis and visualization is carried out.
This includes:

•	a horizontal bar plot to compare the difference in the number of incidents by crime type between 2005-2006 (first years record in dataset) and 2016-2017 (last years record in dataset).

•	a bar plot showing the number of incidents recorded per year (with bar colour indicating whether incidents for a specific year where above or below the mean number of incidents for the entire dataset). 

•	Scatter plots for each individual crime type over time, to visualize change over time for individual crime categories.

•	By inputting a specific Province, the above plots are repeated, however allowing the user to further analyse this data at a provincial level, e.g. Data for Western Cape only.

•	The Provincial analysis is expanded on by using simple linear regression to evaluate general trends in the data. Due to the large variation in the number of and range of incidents between crime categories, the number of incidents has been normalized to allow for analysis of relative change over time. 

•	Results of the linear regression model are then used to generate: (1) a list of all Crime Types that increased in the specified Province (models with a positive slope), (2) a list of all Crime Types that decreased in the specified Province (models with a negative slope), (3) Finding the Crime Type that showed the HIGHEST relative INCREASE in the Province (as inferred from slope sign and value), (4) Finding the Crime Type that showed the HIGHEST relative DECREASE in the Province (as inferred from slope sign and value), (5) Finding the Crime Type that showed the LOWEST relative INCREASE in the Province (as inferred from slope sign and value), (6) Finding the Crime Type that showed the LOWEST relative DECREASE in the Province (as inferred from slope sign and value), (7) Finding the Crime Type that showed the most consistent increase year after year (as inferred from the R-squared value), and (8) Finding the Crime Type that showed the most consistent decrease year after year (as inferred from the R-squared value).
