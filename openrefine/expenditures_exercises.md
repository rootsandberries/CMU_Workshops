##Cleaning Messy Data with OpenRefine
###Personal consumption expeditures dataset

* Importing a spreadsheet of data into OpenRefine 
* Performing basic clean-up functions like trimming whitespace and deleting columns
* Filtering and faceting data
* Transposing data from wide to long format
* Exporting a dataset from OpenRefine





5. In the Project name box, give the project a name of your choice. Click Create Project.

2. **Remove the blank columns:**. Look for the pull down menu for the column named “Column”. From the pull down menu, select
3. **Change a column name:** Click on the pull down menu for the column name "GeoName". Under Edit Column, choose Rename this Column. Rename the column to "State" and click OK.
3. **Fill down data:** We want to fill the entries down in the State column so that all rows have a state associated with them. From the State column pull down menu, select Edit Cells -> Fill Down. In the top toolbar, click next a few times in order to look at a few pages of results. Verify that the fill operation seems to have worked.



#####Activity 1: In addition to the text facet on State, add another text facet on the expenditure column. Using the facets, view the Pennsylvania, West Virginia and Ohio data for "Gasoline and other engery goods" expenditures.  Which state spent the most per capita in 2017?


> * For each state, for each expenditure type, we now have 8 separate rows, one for each year. Notice the dataset now has 9792 rows, compared to 1227 before transposing. It has fewer columns, but many more rows – this is why it is referred to as a “long” format. Long format can be useful for certain types of data analyses, where all your data measuring the same thing (e.g., per capita expenditures) need to be in one column instead of spread over many.


