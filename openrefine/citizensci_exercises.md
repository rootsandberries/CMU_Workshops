##Cleaning Messy Data with OpenRefine
###Citizen science dataset

* Create a new project from the citizen science dataset and use the clustering feature
* Export a JSON script to perform the same process on another dataset

1.  **Start a new project:** Start up OpenRefine (if it isn’t running) or click on the OpenRefine logo on the top left to go to the main screen. Note: If you were working with another project, it has been automatically saved in OpenRefine and the files are stored locally on your computer. You can see your project listed here and can use Open Projects to go back to it later. 
2. **Import your dataset:** Click on Create Project and import the citizenscience.csv file. Maintain the default settings, rename your project and click Create Project. You should see that there are 1991 records in our dataset. Click on show 50 rows to show more rows displayed in the window.

#####Use the clustering feature to make your data consistent 

1. **Create a text facet:** Go to the species guess column (where our citizen scientists have made a guess as to what species they have observed). From the species_guess column pull down menu, select Facet->Text facet. 
2. **Examine your data:** You'll see that some of them are a bit unusual, and in those cases, you may want to edit them; however, in other cases, you'll see that there are two facets that look very similar, but just have different capitalization, such as American Pokeweed. When we have facets that look similar, we can use OpenRefine's clustering features to help improve the consistency of the values in that column. Click on the Cluster button at the top of the facet window.

#####Concatenate columns in the dataset

#####Actvity 3: Concatenate the scientific_name column with the common_name in parentheses into a new column called Descriptive Name. The format should be \<scientific_name> (<common_name>). 


#####Restructure the dataset by removing columns and rows, and then work with Undo/Redo to roll those changes back
3. **Use facets to define and flag a subset:** From the license column pull down menu, select Facet->Customized facets- >Facet by blanks. Click on true to show only the rows where that column is blank (i.e., rows where no license has been specified). From the quality_grade column pull down menu, select Facet->Text facet Select the casual facet. Now we have a subset of rows that have a blank for license and are casual observations. Let's say that these 18 rows were no good to use. We could flag them (or star them or remove them). From the All column pull down menu, select Edit rows->Flag rows
4. **Remove flagged rows:** Reset all facets by clicking on the Reset All button on the left above the facet windows. Now you should see all the rows in your dataset again, some are flagged and some are not. Later if you decide that you want to remove those flagged rows that you were unsure of, you can. From the All column pull down menu, select Facet->Facet by flag and then select true from the facet window to show only your flagged rows. You can delete all of them. From the All column pull down menu, select Edit rows->Remove all matching rows. All the flagged rows should now be removed from the dataset. Reset all facets again by clicking on the Reset All button on the left above the facet windows to see your remaining rows.
 
> * Note: If you go back to a previous step (like we’ve just done), and then start making new changes/transformations - all the subsequent steps will be deleted permanently.

