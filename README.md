# Chicago Food Inspection

# Abstract
Everybody wants to enjoy a meal without having to worry about health hazards.  
From the Chicago Food Inspection dataset, we would like to know if there are some places to avoid like plague, if going away from touristic points of interest will guarantee a meal done in a well-maintained kitchen with fresh uncontaminated food or if we may have a plate with already bitten by a rat because we went to eat a kebab near Chicago's shore on a nice Summer day. 
Providing the consumers tools to verify the sanitization of a food-related shop may be an interesting addition for some restaurant bookers like TheFork is the main motivation behind this project. 

# Research questions
* What are the most common violation to fail an inspection and the weight of them in the verdict?
* How franchises (Subway, MacDo, ...) differ from "normal restaurants"?
* How much does inspection's frequency depends on previous pass/fail results.
* Does [Chicago's rodent invasion](https://southsideweekly.com/i-smell-a-rat/) influence the number of rodent-related violations?
* Which violations are the most common (in general, by period of the year or location)?
* Are violations related to location (ie touristic vs residentential, old vs new district)?
* Can we rank restaurants based on some (still not found) rules?
* Are the 'out of business' restaurants more likely to have failed inspections in the past?

# Dataset
We will be using the [Chicago Food Inspections](https://www.kaggle.com/chicago/chicago-food-inspections#food-inspections.csv) dataset. For our analysis, it requires some modifications:
* Remove columns that are empty (Community Areas, Zip codes, Historical Wards) or redundant (State column only contains IL).
* Normalize shop names by removing numbers (ie WALGREENS #10771 -> WALGREENS) for easier grouping of licensed stores.
* Flatten/explode the violations after parsing them.
* Add a distric (and/or community area and/or ward) column to have new means of grouping. This can be done using the Chicago geospatial data in Geojson from [here](https://data.cityofchicago.org/Facilities-Geographic-Boundaries/Boundaries-Neighborhoods/bbvz-uum9).  
  
Displaying our results will mostly be achieved with maps. For example an interactive map showing the failed/passed inspections over time. We expect to find a lot of differences between districts 

# A list of internal milestones up until project milestone 2
First week:
* Download the dataset and initialise the environment 
* remove the columns that ar empty or redundant. (useless column)
* Normalize shop names by removing numbers
* Flatten/explode the violations after parsing them
* add a distric column

Second week:
* Make the first analysis with histograms
* Implement the aggregation to plot median,sum, mean, ...

Third week:
* Go deeper in the analysis
* Use statistical tools to show important result (correlation, ... )
* Begin to make conclusions about what we found
* Make sure that the stats ar relevant
* Test the hypothesis (p-values)

Fourth week:
* Finalize the conclusions and add comments where needed
* Tidy up the notebook
* Clean the plots, make them conclusive, add error and incertainty, ...
* Write a final conclusion


# Questions for TA
Add here some questions you have for us, in general or project-specific. 
