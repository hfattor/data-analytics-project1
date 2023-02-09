# Starchasers Data Analytics

This study addresses the relationship between the change in a state's population and its population density, and the number of unidentified flying object (UFO) sightings reported. 

## Data Sources

U.S. census data is used to determine state populations and state population density rankings. These data are gathered every 10 years.

Reports of UFOs were gathered from a dataset published on Kaggle (https://www.kaggle.com/datasets/NUFORC/ufo-sightings) by the National UFO Reporting Center (NUFORC). These data were divided into decades based on the year in which they were reported, in order to assess UFO reports within the 10 years of the U.S. census data. The dataset ran from 1950-2013. 

Data before 1950 and after 2010 was removed from this data analysis in order to present full decades of data across the two datasets.

## Focus States

Analysis further focused on 11 states that had the highest number of UFO sightings reported:
<ul>
    <li> Arizona: 3,414 sightings</li>
    <li> California: 8,912</li>
    <li> Florida: 3,835</li>
    <li> Illinois: 3,499</li>
    <li> Michigan: 1,836</li>
    <li> New York: 3,980</li>
    <li> Ohio: 2,275</li>
    <li> Oregon: 1,747</li>
    <li> Pennsylvania: 2,366</li>
    <li> Texas: 3,447</li>
    <li> Washington: 3,966</li>
</ul>

By focusing the study on these 11 sample states with a higher number of UFO sightings reported, analysis examined consistently high reporting data across 60 years and compared state population density to these reports. Maps of each state are available in the 'Output/State Maps' folder. These maps present the location of each reported UFO sighting in a state, with the color representing the year the sighting was reported. The maps are available as .html files that can be zoomed in and out.

Analysis also looked at the number of UFO reports given in each of the 11 focus states every year during the 60-year period. These are available as bar graphs in the 'Output' folder in a .png format. 

## The 1994 Question

During explorations of the number of sightings per year from the 1950s forward, it was briefly considered to split observations between one of several noted 'jumps' in the total number of sightings annually: Until 1993, there were around 100 sightings per year on average. Then, after 1994, the sightings would steadily increase per year, until 1999 where over 1200 sightings were recorded, continuing at this new increased rate until 2008 where we have almost 2300 sightings.

It was presumed there might be some 'confounding variable' which might statistically skew the results in testing, so the data was initially split into sightings Pre-1994 and sightings Post-1994, inclusive. However, upon further inspection and review, it was concluded this phenomenon is likely due to:
    a) the launching and upkeep of the NUFORC.org website, which has been in operation since 1994, and
    b) the increased access to reporting technologies such as mobile devices, allowing more individuals to access NUFORC via telephone line and potentially web.
    
After consideration of the above factors, there was no indication that these phenomena would affect our samples in question disproportionately. Further discussion and quantitative reasoning in 'Analysis'.

## <em>Hypothesis: If a state experiences a rise in population, then the number of UFO sightings reported will also increase.</em>

## Analysis - Correlation and Regression

This study explored the change in a state's population every decade (as recorded by the U.S. Census) and the number of UFO sightings reported during that 10-year timespan. A scatterplot of this data is available in the 'Output' folder in a .png format. The limited availability of year-by-year census data limits how tightly these factors can be correlated, but this is due to data availabilty regarding the U.S. population.

In the U.S. Census' definition, population density is "a measure of average population per square mile." If a state had a resident population density over 100, it was classified as a high-density state for this analysis. If a state had a resident population density under 100, it was classified as a low-density state. 

Of the 11 focus states, 8 were high-density during periods of the 60-year span we looked at (California, Florida, Illinois, Michigan, New York, Ohio,  Pennsylvania, and Washington) and 7 were low-density during periods of the 60-year span we looked at (Arizona, California, Florida, Oregon, Texas, and Washington).

This analysis found a very weak positive correlation between the number of UFO sightings reported and resident population density for high-density states (r-value: 0.117773). Low-density states have a slightly higher positive correlation between the number of UFO sightings reported and the resident population density (r-value: 0.263391). A scatterplot of each of these state population categories, including the line of best fit, can be found in the 'Output' folder in a .png format. The conclusion of this study is that there is very little correlation between the two variables, and therefore the alternative hypothesis presented above is disproven.

## <em>Null Hypothesis: There is no difference in the samples of UFO sightings recorded between states with high population density and states with low population density.</em>

## Analysis - T-test

In a two-sample T-test, this study found that, using a standard alpha value of 0.05, the p-value between sightings reported per year in high-density states vs. the sightings per year in low-density states was low (p-value: 0.024994). Therefore, this study successfully rejects the null hypothesis and suggests the two samples of sightings per year have a statistically significant difference. That is to say, low-density states and high-density states report a difference in the statistical spread of sightings per year, and by measures of central tendency.

# Further Research

It is intriguing to note the instances of cities and states which reported high numbers of sightings in total compared to what their relative populations were. For instance, Portland, OR ranks among the top five cities which report the most number of sightings across the years, but as of 2014 ranked as only the 28th most populated city in America (U.S. Census Bureau). Many more variables are at play which may contribute to such focused and/or vast distributions in the accumulation of UFO sightings.

Because of the magnitude of data, focus was put on specific states and statewide populations. Any future study of this topic may focus on areas of states (e.g., counties, census tracts, cities) that had high-density UFO reports across decades. These areas would be determined by longitude and latitude reported to the NUFORC. Examples of these areas for further study can be found in the 'Output/State Maps' folder. These .html maps note the location of each reported UFO sighting in a state, with the color representing the year the sighting was reported. As another example, further study could look into aircraft sites within 50 miles of high UFO-sighting sites and examine a relationship there.

Because there are spikes of increased UFO sighting reports in specific years that span the 60-year timeframe this study examined, any further study may consider what other factors during these years might affect UFO reports. For example, NASA has data on fireballs (celestial anomolies such as meteor showers) over the years. Comparing fireball sighting locations to UFO reporting sights may show a relationship between the two. The years that may warrant further study can be found by looking at the bar graphs in the 'Output' folder.
