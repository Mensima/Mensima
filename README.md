# (Ford Gobike System Data Exploration)
## by (Samantha Erskine)


## Dataset

>  This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area in the month and year of February 2019. It contains 183412 columns and 16 rows, and is stored in a csv file. Columns include duration_sec, start_time, end_time, start_station_id, start_station_name, start_station_latitude,start_station_longitude, end_station_id, end_station_name,end_station_latitude, end_station_longitude, bike_id, user_type,
member_birth_year, member_gender, and bike_share_for_all_trip.


## Summary of Findings
### Data Wrangling
> After importing the necessary packages for this exploration, the data had to be wrangled before stepping into the visualisation process. Numpy, pandas, matplotlib.pyplot andseaborn as well as, %matplotlib inline were imported. The ford go bike share system for February 2019 data set was loaded. In the wrangling process, the dataset was investigated further using functions to show info and datatypes, check for null values and duplicated values. After this, in order to initiate the cleaning while maintaining the original dataset a copy of the dataset was made called gobike_clean. In the wrangling assessment, it was determined that changing the duration in seconds column to minutes would be better for visualization exploration, and so this was done, columns that were not directly worked on were also removed these are, start_station_latitude,start_station_longitude,end_station_latitude,end_station_longitude, and duration_sec' . There was no column indicating the ages of members, however their birth years were indicated and was subtracted from the current year to get their ages. The member_birth_year column which was originally a float was changed into an int datatype. A categorical sectioning of the age of members were made, People 0-30 years old were categorized as young, 31-60 was described as middle aged and 61-150 were described as old, for further analysis. Before the univariate data analysis begun, a function was defined to make formatting of visualizations easier.


### Univariate data exploration
> In order to explore the variables of interest individually, some univariate visualizations were made. First, the labelled bar chart of the gender of member, male, female and other genders. After this, a donut pie chart was created to assess the user type that members opted for, which are subscribers or customers. Next a histogram of the duration of bike rides in minutes. The histogram was largely focused arounf 0-100 minutes and so a visualization was made highlighting those number of minutes. Next, a histogram of the age of members was created. After this, a pie chart was made to investigate how many people chose to use the bike for a full trip or not, with a legend of yes and no. This ends the univariate analysis.


### Bivariate data exploration
> In the bivariate exploration the features of interest were measured against each other. The first visualization shows the relationship between gender and the duration of minutes ridden on bikes in a scatter plot and a box plot in subplots. The next visualization shows the relationship between the user type members opted for and whether or not they chose to use the bike for a full trip. Next, the next relationship explored was that of the age group the members have been categorized into against the duration of minutes they rode their bikes in a scatter plot, and the age of members against the duration of minutes they rode their bikes in a histogram in two subplots. The next exploration showed the relationship between age group of members and whther or not they opted to use the bikes for a complete trip in a stacked histogram. Next the relationship between which user type members chose and the duration of minutes ridden on bikes in a histogram. The next relationship explored was between age group of members and user type in a stacked bar chart.


### Multivariate data exploration
> In the multivariate exploration, more than two features are measured against each other to gain more insight. The first visualization here shows the relationship between age group of members, which user type they opted for and the duration of minutes in which they rode bikes in a box plot with a legend. The next visualization shows the relationship between the gender of members, the age group of members and the duration of minutes in which they rode bikes in a facetgrid. Next, a heatmap shows the relationship between the age group of members, whther they used bike share for a full trip and the duration they rode the bikes for. Finally, a lineplot indicates the relationship between members' preferred user type, birth year and the duration of minutes the in which the bike was used.

## Key Insights for Presentation

> In this section, I will highlight one of my features of interest, which is seen to be the age group of members, and how this feature shows more insight as it is compared against other features which are the duration of bike rides in minutes and the user type. This will be shown in three visualizations, one univariate, one bivariate and one multivariate.