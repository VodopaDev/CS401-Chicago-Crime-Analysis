# Title

# Abstract
A 150 word description of the project idea, goals, dataset used. What story you would like to tell and why? What's the motivation behind your project?

# Research questions

* Investigate what are the most common reasons to fail an inspection and the weight of them in the verdict.
* Are violations related to location (ie touristic vs residentential, old vs new district, rich vs poor)? This can be visualized with a (pretty) map thanks to the latitude/longitude and additional data ([wealth](https://www.chicagobusiness.com/static/section/chicagos-wealth-divide.html), [zoning](https://gisapps.chicago.gov/ZoningMapWeb/?liab=1&config=zoning)).
* Compare how franchises (Subway, Macdo, ...) differ from "normal restaurants".
* How much does inspection's frequency depends on previous pass/fail results.
* Are there some restaurants that "escape" food inspections?
* Compare rodent-related violations to [Chicago's rodent invasion](https://southsideweekly.com/i-smell-a-rat/)
* See if there was any law (from the USA, IL or Chicago) that may have influenced the result of inspections

* Analysis on the different 'violations':
* - Which violations are the most common ?
* - Are there locations/periods where a certain type of violation is more common ?

* Construct an interactive map showing the failed/passed inspections over time (with a scroll bar for example). Same for the risk levels can be done.
* Construct some rankings of the 'restaurants' based on different rules.
* Are the 'out of business' restaurants more likely to have failed inspections in the past ?

# Dataset
We will be using the [Chicago Food Inspections](https://www.kaggle.com/chicago/chicago-food-inspections#food-inspections.csv) dataset.  
* Remove useless columns that are empty (Community Areas, Zip codes, Historical Wards) or redundant (State column only contains IL).
* Normalize shop names by removing numbers (ie WALGREENS #10771 -> WALGREENS) for easier grouping of licensed stores.
* Flatten/eplode the violations after parsing them.
* Add a distric or community area column to have new means of grouping. This can be done using the Chicago geospatial data from [here](https://data.cityofchicago.org/Facilities-Geographic-Boundaries/Boundaries-Neighborhoods/bbvz-uum9).
List the dataset(s) you want to use, and some ideas on how do you expect to get, manage, process and enrich it/them. Show us you've read the docs and some examples, and you've a clear idea on what to expect. Discuss data size and format if relevant.

# A list of internal milestones up until project milestone 2
Add here a sketch of your planning for the next project milestone.

# Questions for TAa
Add here some questions you have for us, in general or project-specific. 
