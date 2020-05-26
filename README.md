# ActivityDoubtResolution
Assignment Implementation Notes:  

1. Added a new Column user_type based on the activity_type of the user_id

2. Added a new Column TA_Count based on user_type TA for each doubt_id resolved/worked upon. This lets us know the number of TAs working on the given doubt. 

3. Using GroupBy and Merging to get dataframes with respect to Doubt and Activity dataframes with the additional columns described above.

4. Getting the doubt Resolution time by converting the datetime string to python datetime object and localizing the timezone to None. 

5. Getting correlations between the columns resolution time and the user rating to get the relationship between the two. 

6. Using correlations between the columns TA_Count and the resolution time and the user rating pairwise to get the relationship between the two. 

7. Getting the other relationship between the column doubt category and the doubt resolution time as to which doubt category is taking more doubt resolution time through groupby query and barplot visualization for the specific course. 

8. For False positive doubts or cleared doubts, TA was not required so the user rating is not given and the resolution time is minimal.

Extracted information and the inferential data have been dumped into the csv file generated through the python notebooks. Library Used: pandas, numpy, seaborn
