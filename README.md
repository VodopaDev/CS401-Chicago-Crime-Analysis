# Title

# Abstract
A 150 word description of the project idea, goals, dataset used. What story you would like to tell and why? What's the motivation behind your project?

# Research questions
* What are the most common reasons to fail an inspection and the weight of them in the verdict?
* How franchises (Subway, MacDo, ...) differ from "normal restaurants"?
* How much does inspection's frequency depends on previous pass/fail results.
* Does [Chicago's rodent invasion](https://southsideweekly.com/i-smell-a-rat/) influence the number of rodent-related violations?
* Which violations are the most common (in general, by period of the year or location)?
* Are violations related to location (ie touristic vs residentential, old vs new district, rich vs poor)?
* Can we do rankings of the restaurants based on some (still not found) rules?
* Are the 'out of business' restaurants more likely to have failed inspections in the past?

# Dataset
We will be using the [Chicago Food Inspections](https://www.kaggle.com/chicago/chicago-food-inspections#food-inspections.csv) dataset. For our analysis, it requires some modifications:
* Remove columns that are empty (Community Areas, Zip codes, Historical Wards) or redundant (State column only contains IL).
* Normalize shop names by removing numbers (ie WALGREENS #10771 -> WALGREENS) for easier grouping of licensed stores.
* Flatten/explode the violations after parsing them.
* Add a distric (and/or community area and/or ward) column to have new means of grouping. This can be done using the Chicago geospatial data in Geojson from [here](https://data.cityofchicago.org/Facilities-Geographic-Boundaries/Boundaries-Neighborhoods/bbvz-uum9).  
  
Displaying our results will mostly be achieved with maps. For example an interactive map showing the failed/passed inspections over time. Same for the risk levels can be done.
  
List the dataset(s) you want to use, and some ideas on how do you expect to get, manage, process and enrich it/them. Show us you've read the docs and some examples, and you've a clear idea on what to expect. Discuss data size and format if relevant.

# A list of internal milestones up until project milestone 2
Add here a sketch of your planning for the next project milestone.

# Questions for TAa
Add here some questions you have for us, in general or project-specific. 
