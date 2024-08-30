***A Guided Exploration of UN Data (Gross Domestic Product and Internet Usage)***

**Project Overview**:

This project involves analyzing two datasets: Gross Domestic Product (GDP) per capita and Internet usage. The analysis will be conducted using Python and Jupyter Notebook, focusing on data cleaning, exploration, and visualization.

***Technology Used***: Jupyter Notebook (Python)

**Getting Started**:

1. Create a Data Folder

	Create a folder named data in your local project repository.

2. Download and Prepare Datasets

	**Gross Domestic Product (GDP) per capita**:

	Download from [UN Data](https://data.un.org/Data.aspx?d=WDI&f=Indicator_Code%3aNY.GDP.PCAP.PP.KD) without applying any filters. Rename the file to gdp_percapita.csv. Open it with a text editor to review the content.

	**Percentage of Individuals Using the Internet**:

	Download from [UN Data](https://data.un.org/Data.aspx?d=ITU&f=ind1Code%3aI99H) without applying any filters. Rename the file to internet_use.csv. Open it with a text editor to review the content.

3. Set Up Jupyter Notebook
   
	Create a folder named notebooks and launch a Jupyter Notebook in this folder. Name it appropriately.

***Data Analysis Steps***:

**GDP Dataset**:

1. Load the Data
   
	Import the GDP dataset using pandas.read_csv() into a DataFrame called gdp_df. Examine the first and last few rows to familiarize yourself with the data.

2. Data Cleaning
   
	Determine the number of rows and columns in gdp_df and check the data types of each column. Drop the "Value Footnotes" column and rename the remaining 		columns to 'Country', 'Year', and 'GDP_Per_Capita'.

3. Data Analysis

	Find the number of countries with complete data and identify countries with missing data.

	Analyze the number of observations per year.
4. Visualizations for 2020

	Create and compare histograms, density plots, boxplots, and violin plots for GDP per capita in 2020.

5. GDP Trends Over Time

	Subset the data for the years 1990, 2000, 2010, and 2020 into a new DataFrame gdp_decades. Create and analyze boxplots, barplots, scatterplots, and scatterplots with trend lines.

**Key Insights**

  Identify the first country to exceed $100,000 in GDP per capita.
 
  Determine the country with the highest GDP per capita in 2020 and visualize its GDP changes over time.
 
  Find the country with the lowest GDP per capita in 2020 and visualize its GDP changes over time.

  Bonus: Compare GDP per capita between 1990 and 2020 to identify countries with lower GDP in 2020.
 
**Internet Usage Dataset**

1. Load the Data
   
	Read the internet usage dataset into a DataFrame named internet_df. Check and correct any errors during import, then review the top and bottom rows and data types.

2. Data Cleaning
   
	Drop the "Value Footnotes" column and rename the remaining columns to 'Country', 'Year', and 'Internet_Users_Pct'.

3. Data Analysis

 	Examine the number of observations per year.
 
 	Identify the first year with a non-zero internet users percentage.
 
4. Visualizations for Internet Usage

 	Compare the distribution of internet users' percentage for the years 2000 and 2014.

	 Determine how many countries had less than 5% internet usage in 2014.
 
**Merging and Further Analysis**
1. Merge DataFrames

 	Merge gdp_df and internet_df into a new DataFrame called gdp_and_internet_use. Ensure that the merge keeps all rows from both DataFrames.

2. FacetGrid Visualization

	 Find the top three countries with the highest internet users' percentage in 2014. Use Seaborn's FacetGrid to compare GDP changes over time for these countries.

3. 2014 Data Analysis

 	Subset gdp_and_internet_use for the year 2014 and save it as gdp_and_internet_use_2014. Create a plot comparing Internet Users Percentage and GDP per Capita for 2014 and investigate any unusual points.

Feel free to reach out with any questions. Happy analyzing!

This project was completed as part of an apprenticeship with Nashville Software School.
