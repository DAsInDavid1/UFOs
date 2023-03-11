# UFOs
Analysis of UFO sightings and visualizing it using JavaScript to create a webpage

## Overview of Project
The purpose of this webpage was to allow users to filter through the sightings of UFOs over the world and filter based off date, city, state, country, or shape. This would allow the users to have an indepth experiance on the webpage and let them see which data they would like.

## Results
The webpage works very simply. When someone enters a filter on the left hand side that matches the data in the dataset then it will only show the data that matches the filter. 

In the code when someone puts in something into the filters, it will save the element that was changed, save the value of the element, and save the id of the element that was changed. 

<img src= "https://github.com/DAsInDavid1/UFOs/blob/main/static/images/saving_elements.png" width=50% height=50%> 

Once the filter is entered we use a if/else statement to determine that if a filter was entered then the key [id] in the variable "filters" would be matched to the value of the filter, making a key:value pair. If no filter was entered or deleted, then the filters key [id] would be deleted.

<img src= "https://github.com/DAsInDavid1/UFOs/blob/main/static/images/if_filter_was_entered.png" width=25% height=25%> 

Next the code uses the funcion "filterTable" to change the data rows to only match what filter was entered. We use a forEach statement on the filters variable, and for each key:Value pair in the filters variable it filters the rows of the table to make the key:value pair match with the rows and apply it to the variable filteredData to built our new table.

<img src= "https://github.com/DAsInDavid1/UFOs/blob/main/static/images/filteredData.png" width=50% height=50%> 

## Summary
This webpage could be more optimized for user experience. The user must manualy type in the filter criteria, which if they mistype then no tables will show up as seen with the example below.

| Triangle spelled correctly  | Triangle spelled wrong
| ------------- | ------------- 
| <img src= "https://github.com/DAsInDavid1/UFOs/blob/main/static/images/triangle_filter.png" width=100% height=100%>   | <img src= "https://github.com/DAsInDavid1/UFOs/blob/main/static/images/triangl_filter.png" width=100% height=100%>   

The biggest drawback is currently the ability for the user to misspell,wrong capilization, or typing incorrectly  will bring no results for the filter.

I would recomened that a drop down menu be implemented for the filters so that when someone types in something, a recomened filter from the drop down must be clicked so that the filter works. Another recomendation to solve this issue would be to implement a "error" code where when someone types in a filter that doesnt show data a error message pops up telling them to either correct their filter or try something else.

Another rocomendation would be to allow the user to extract the data from the website in a JSON format so that once they filter the data how they want, it can give them a file of usable data for them to analyse deeper if the user wished to.
