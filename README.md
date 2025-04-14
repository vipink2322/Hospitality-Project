# Hospitality-Project
This project describe the hospitality in Atlias Group of Organization
### Week-on-week (WOW)
Week-on-Week (WoW) is a type of business metric that measures changes in a specific variable over a period of one week compared to the previous week. It is a common way of tracking business performance over time and is particularly useful for analyzing trends and identifying areas where improvements can be made.
Here are the metrics for which we found the WoW change:
1. Revenue WoW change %: To get the revenue change percentage week over week.
2. Occupancy WoW change %: To get the occupancy change percentage week over week.
3. ADR WoW change %: To get the ADR (Average Daily rate) change percentage week over week.
4. RevPAR WoW change %: To get the RevPAR (Revenue Per Available Room) change percentage week over week.
5. Realisation WoW change %: To get the Realisation change percentage week over week.
6. DSRN WoW change %: To get the DSRN (Daily Sellable Room Nights) change percentage week over week.



-----------------------------> Data Loading and Power Query Documentation -------------------------------------->


1. Create a folder in Desktop and store all the csv files related to hospitality challenge.

2. Open a Power BI file, and In "Get Data", select the option as folder and browse through the folder containing csv files.

3. Then go to Tranform data to expand each and every dataset.

4. Now, duplicate the data source 4 times and in each one, expand one dataset by clicking on "Binary" option. also, rename 
   the tables accordingly.


*****************  Power Query steps for tables:  *******************
1. dim_date:
	- remove the column 'day_type'
	- we are deleting this because, we got a feedback from the mock dashboard review that Friday and Saturday are           
	  considered as weekends in the industry and not sunday. But In our datasets, saturday and sunday are considered           
	  as weekends. So we delete this column and re-create day_type using calculated columns.

2. dim_rooms
	- The column names are not captured here. We need to select "Use First Row as Headers" option .
