# Adata-project2  
[Chicago Food Inspections](https://www.kaggle.com/chicago/chicago-food-inspections#food-inspections.csv)  
[Chicago Food Inspection WebSite](https://www.chicago.gov/city/en/depts/cdph/provdrs/healthy_restaurants/svcs/food_protection_program.html)  

### Cleaning:

* Remove useless columns that are empty (Community Areas, Zip codes, Historical Wards) or redundant (ie State and City columns only contains IL and CHICAGO respectively).
* Clean shop names for easier grouping.
* Flatten the violations.

### Ideas:

* Investigate what are the most common reasons to fail an inspection and the weight of them in the verdict.
* Are violations related to location (ie touristic vs residentential, old vs new district, rich vs poor)? This can be visualized with a (pretty) map thanks to the latitude/longitude.
* Compare how franchises (Subway, Macdo, ...) differ from "normal restaurant".
* (a bit vague) Analysis of the violations' comments.
* How much does inspection's frequency depends on previous pass/fail results.
* Are there some restaurants that "escape" food inspections?
* Compare rodent-related violations to [Chicago's rodent invasion](https://southsideweekly.com/i-smell-a-rat/)
* See if there was any law (from the USA, IL or Chicage) that may have influenced the result of inspections
