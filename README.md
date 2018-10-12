# project-one---sphinx
QUESTION -	What types of causes receive the most money?

This notebook looks at the correlation between the type of donation and the amount of money given. It features two main graphs, showing the total amount of donations for 2015 - 2018 broken down by cause type and the yearly change in donation amounts for the top five highest earning causes over the course of four years.

The data was pulled from the Chronicle of Philanthropy, put into four seperate csv files and read into the notebook for analysis. It revealed that the top five recent highest earning causes are:

Colleges and universities 
Health 
Foundations 
Arts
and Community foundations

Colleges and universities is by far the highest earning cause, with a four year total of over $20 billion. There was also an interesting uptick in the donations to foundations in 2017, with a massive uptick from roughly half a billion in 2016 to 4 billion in 2017 and then a return to about half a billion in 2018. Health also saw an uptick in donations in 2017, growing from 1 to 2 billion from 2016 - 2017. 

NOTE: 2018 donation numbers will be lower than final numbers as the year has not ended yet. 

QUESTION - What is the correlation between donor source of wealth and amount of money given over the course of recent years? 

With regard to the correlation between donor source of wealth and amount of money given over the course the four years 2015 to 2018:

The largest donation of $1.8 billion was made to a Chan Zuckerberg Foundation from Mark Zuckerberg and Priscilla Chan in 2017. Their source of wealth was in Technology. Notably their residence of California is of no surprise.

The wealth category groupings were bucketed to allow for distinction among 192 unique strings of 2 or more sources of wealth. This created 13 distinct categories and these were used to identify wealth source. A separate csv cross reference file was created and saved to the master repository.

Overall 95% of all donations came from Technology followed by Manufacturing, Family Wealth and Real Estate.

There was a relationship found with a donors source of wealth and their donation amount. Wealth categories that command more value in the market yielded higher donations. Healthcare and Retail sources of wealth yielded nearly identical amounts of donations over the 4 years with Transportation and Education being the lowest. 

QUESTION - What is the geographic concentration of Philanthropy? How can this be mapped?
Unsurprisingly, the highest concentration of donors and recipients were in larger population centers.  
There was a fair amount of regional loyalty, many donors from a state often gave to organizations in their same state. 
The raw data only contained state level geographic information.  In order to use GMAPs there needed to be latitude and longitude coordinates. The existing dataframe was merged with another source of geographic coordinates by state.  These generalized state level coordinates were then mapped using GMAPs to provide a spatial understanding of the location of both donors and recipients.
Matts_Sphinx.ipynb with 1000-largest-us-cities-by-population-with-geographic-coordinates.csv, cop_gifts_1518_20181011.csv, statelatlong.csv, plus chronicle_data2015-2018.csv
NOTE: my code uses " from config_googlemaps import gkey " modify your config file for google maps as needed.

Data Sources:https://www.philanthropy.com
https://www.kaggle.com/washimahmed/usa-latlong-for-state-abbreviations  https://public.opendatasoft.com/explore/dataset/1000-largest-us-cities-by-population-with-geographic-coordinates/information/?sort=-rank&basemap=jawg.streets&location=3,44.55855,-114.05683

QUESTION? - How have total amount of donations changed in the last 4 years?
Based on the graphical representation of the Annual calculations of total donations, the highest amount of donation from all donors was made in 2017. However, as demonstrated by the graph it should me noted that there is a gradual increase in donation amount between 2015 and 2017 and although 2018 currently has the lowest total amount of donations, the year isn't over yet, and the data obtained on donations for the years 2015 through 2018 don't include details about the months, dates or days on which donations were made - a limitation faced in analysing our data
