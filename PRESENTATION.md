# Presenting the results of Coursera's Project

# Introduction
For Coursera's Applied Data Science Capstone project, I deliver this markdown file as a means to present the findings that were made as we applied the project.
For the sake of giving an insight onto the project matter, we introduce the project as: helping to recognize the data set of venues located in Paris, by Arrondissement, and finding out whether Rabat, Morocco's Hay Riad district is somewhere close to resembling one of the Arrondissement in Paris, in that way solving for why the prices of rent are too high there.

# Chosen Data
Foursquare offers a lot of insight into what kinds of venues can be found in a specific area:
* [Cuisine] Restaurant, of many such as French, Japanese, American...
* Hotels,
* Parks,
* Zoos,
* and others...

With those data and the data pertaining to Paris in a geojson format, we can get some insight into what kind of areas are Paris's and in what way our sole city moroccan chic housing area is close to any specific arrondissement of Paris

# Methodologoy
What we did, is fix a position for each Arrondissement of Paris based on a geojson map. We get for each Arrondissement a specific point of interest, where the location is mainly a center of mass of the geojson specific Polygon. From these we set centers of every Arrondissement and we are ready to apply similar exploration techniques as done in the Course handout. We gather for 20+1 center the venues in the vicinity of points chosen, and use their categories as a basis for clustering the data. The most common types of venues are set to each data point, and we aim to differentiate them in 5 clusters.

# Results
Much to our surprise, the moroccan area chosen was out of all clusters pertaining to Paris, displaying a high presence of Food Venues mainly. That is not the case of our French datasets, which display a more variate surrounding. Some areas lack in number of venues as well. What distinguished Paris is a clear bias between Eastern and Western halves of it. The western area comprised two different clusters, mainly rich (7th and 16th Arrondissement), and less rich areas (14th, 15th, 8th, 17th).
All other areas were found as displaying the same features. What differentiates rich areas is the presence of Gardens as 4th level of presence. And what makes 12th Arrondissement as a peculiar type is the presence of zoos.

# Discussion
Maybe the low usage of Foursquare is the source of bias in the moroccan dataset since only restaurant venues seem to appear in the area. We won't jump to conclusions, but the quality of the data show that this area, not unlike others remains in the mainstream quality of "Food, food, more food..." behaviour that is seen in many areas. Unless the quality of restaurants is high, there's no reason for a particular spot to be wealthier than any other spot.

# Conclusion
Not much to our expectations, the moroccan area did not fit into the clustering made in Paris. Thus is no way similar to it. It is developing and not developed, yet it displays unbalanced wealth just based on the quality of restaurants that are available there.
