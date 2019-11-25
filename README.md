# Chicago Food Inspection

# Milestone 2  

The notebook to look at is milestone2.ipynb!

# Milestone 1  

## Abstract
Everybody wants to enjoy a meal without having to worry about health hazards.  
From the Chicago Food Inspection dataset, we would like to know if there are some places to avoid like plague, if avoiding touristic points of interest will guarantee a meal done in a well-maintained kitchen with fresh uncontaminated food or if we would have a dish already bitten by a rat because we went to eat a kebab near Chicago's shore on a nice summer day. 
Providing consumers with tools to verify the sanitization of a food-related shop may be an interesting addition for some restaurant bookers like TheFork. This is the main motivation behind our project. 

## (Main) Research questions
* Does [Chicago's rodent invasion](https://southsideweekly.com/i-smell-a-rat/) influence the number of rodent-related violations?
* Which violations are the most common (in general, by period of the year or location)?
* Are violations related to location (ie touristic vs residentential, old vs new district)?

## Dataset
We will be using the [Chicago Food Inspections](https://www.kaggle.com/chicago/chicago-food-inspections#food-inspections.csv) dataset. For our analysis, it requires some modifications:
* Remove columns that are empty (Community Areas, Zip codes, Historical Wards) or redundant (State column only contains IL).
* Normalize shop names by removing numbers (ie WALGREENS #10771 -> WALGREENS) for easier grouping of licensed stores.
* Flatten/explode the violations after parsing them.
* Add a district (and/or community area and/or ward) column to have new means of grouping. This can be done using the Chicago geospatial data in Geojson from [here](https://data.cityofchicago.org/Facilities-Geographic-Boundaries/Boundaries-Neighborhoods/bbvz-uum9).  
  
[See this for how to find to which polygon a point belong](https://stackoverflow.com/questions/20776205/point-in-polygon-with-geojson-in-python).  
It will be useful to create our district/ward/area columns from the Chicago's Geojson.  
  
Displaying our results will mostly be achieved with maps. For example an interactive map showing the failed/passed inspections depending on the localization. We expect to find a lot of differences between districts and communities.

## An approximate list of intermediate milestones  
  
First week:  
* Download the dataset and initialise the environment  
* Remove the columns that are empty or redundant. (useless column)  
* Normalize shop names by removing numbers  
* Parse and explode/flatten the violations  
* Add a distric column

Second week:  
* Make the first analysis with histograms  
* Implement the aggregation to plot median, sum, mean, ...  
  
Third week:  
* Go deeper in the analysis  
* Use statistical tools to show important result (correlation, boxplot, ... )  
* Begin to make conclusions about what we found. 
* Make sure that the stats are relevant.  
  
Fourth week:  
* Finalize the analysis and add textual descriptions.  
* Tidy up the notebook.  
* Clean the plots, make them conclusive, add error and incertainty, ...  
* Write a final conclusion.  
  
## Questions for TA
* Is our project ambitious enough ? Too ambitious ?
* Does 'providing consumers with safer food-related information' explains some aspect of 'social good' enough? Or is it desirable to ask further and deeper question?
* Do you have bad experiences from a Chicago's restaurant to share with us ?

