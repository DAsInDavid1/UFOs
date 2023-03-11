# UFOs
Analysis of UFO sightings and visualizing it using JavaScript to create a webpage

## Overview of Project
The purpose of this webpage was to allow users to filter through the sightings of UFOs over the world and filter based off date, city, state, country, or shape. This would allow the users to have an indepth experiance on the webpage and let them see which data they would like.

## Results
The webpage works very simply. When someone enters a filter on the left hand side that matches the data in the dataset then it will only show the data that matches the filter. In the code when someone puts in something into the filters, it will save the element that was changed, save the vale of the element, and save the Id of the element that was changed. 

Once the filter is entered we use a if/else statement to determine that if a filter was entered then the key [id] in the variable "filters" would be matched to the value of the filter, making a key:value pair. If no filter was entered or deleted, then the filters key [id] would be deleted.

Next the code uses the funcion "filterTable" to change the data rows to only match what filter was entered. We use a forEach statement on the filters variable, and for each key:Value pair in the filters variable it filters the rows of the table to make the key:value pair match with the rows and apply it to the variable filteredData to built our new table.
