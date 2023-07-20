

# Crime Analysis [![Presentation](https://img.shields.io/badge/Presentation-red?style=flat&logo=codereview)](https://docs.google.com/presentation/d/1TGgtrsVOVzgK9oL2wOtrSuxz2anh69CpDysVYDjF-t4/edit#slide=id.g23188ea39e2_0_61)

### Project description:
This is a group project that included a creation of a workflow in GitHub to collaborate on an observetional study of crime in the city of Chicago, Illinois. The purpose of the analysis and the main reaseach question was **"how did COVID-19 impact crime in Chicago?"** To conclude on this question, the following sub-questions were analysed: 
1. Did covid impact the distribution of crime in Chicago?
2. Did covid impacted the crime types?
3. Has covid had an impact during holiday seasons?
4. Has it impacted the number of domestic crime?
5. Did covid impact how prolific each type of crime is? 

### Project outline
* Finding idea for research.
* Data Collection - APIs and CSVs. 
* Data preperation, cleaning, and manipulation. 
* GitHub workflow creation (workflow planning and implementation -> Methods? How to collaborate? What files should/n't be included etc.., creation of feature branches, merging the feature branches to the main branch). 
* Gathering resources & maps for the research. 
* Data Analysis. 
* Presenting the key findings and conclusions. 

#### Libraries & APIs Used
**Libraries:**
* Pandas
* Os
* ZipFile
* holidays
* Matplotlib
* NumPy 
* Seaborn 
* requests 
* json
* pathlib
* hvplot
* sys
* warnings

**APIs:**
* Geoapify
* Chicago Data Portal


### TLDR - Conclusions 
#### Crime Destribution & Crime Types - Key Takeaways
1. In some Police Districts crime has fallen post-covid, including districts 1, 6, 11 and 18. Whereas in others it has risen, including districts 2, 4, and 12. Thus we can conclude that the distribution of crime within Chicago has changed.
2. Comparing the crime rates in Jan - June 2019 and 2023 with the locations of the police buildings, there is no visible reduction of crime rates in areas where there is a higher concentration of Police buildings (such as the CBD), and also no visible increase of crime rates in areas where there are no Police Buildings (such as South Chicago).
3. While we can say with confidence that crime has been redistributed across the Police Districts of Chicago when comparing 2019 to 2023, we cannot assume any correlation between the COVID-19 pandemic and this redistribution of crime rates. We also cannot conclude that the location of Police buildings has affect where crime was redistributed to.

#### Holiday Seasons - Key Takeaways
1. Inclusive offences that didn’t end up with an arrest:
    1. In general, the COVID-19 period distributed more crime during the “holiday season” than before and post-COVID-19 holiday seasons. 
        1. During COVID-19, Independence Day had the most significant amount of offences; This may as a direct result the George Floyd’s death and the protesting of “black lives matter”.
        2. It may also explain the crime increase during post COVID period over the Juneteenth holiday and the increase in crime on Memorial Day over the post-COVID-19 period.
        3. Christmas had the least offences before COVID-19 and the most significant decrease in crime incidents in all periods. The reason may be that December in Chicago is very cold and is often below freezing. 
2. Offences that did end up with an arrest:
    1. The amount of crime incidents **with arrests** for **during** COVID-19 period and **Prior** to COVID-19 period almost doubled relative to the amount of crime incidents **post COVID-19** period.
    2. Post-COVID-19, Veterans Day holiday had the least amount of crime incidents that ended with an arrest relative to before and during the COVID-19 period.
    3. New Year’s Day, Prior COVID-19 period, had the highest amount of crime incidents with an arrests 
3. Both [NYT](https://www.nytimes.com/article/george-floyd-protests-timeline.html) and [Chicago Suntimes](https://chicago.suntimes.com/news/2021/5/25/22419345/protests-chicago-george-floyd-anniversary-black-latino-unity-racial-reckoning) reported on large amount of protests of “black life’s matter” after George’s Floyd and Anthony’s Alvarez got shot by a police officer which may explain the amount highest amount of crime incidents in a “STREETs”.
4. There were more crime incidents in RESIDENCE and APARTMENTs during and post-COVID-19 relative to the prior period. It may be a direct result of the ramifications of the restrictions and the new reality to be adjusted. 
5. The top 3 community areas that generated crime before, during and after COVID-19 were: Austin, South Shore, and Near North Side. 
    1. According to the following articles from [Chicago Business](https://www.chicagobusiness.com/crains-forum-safer-chicago/chicago-violence-problem-debate-safety-inequality#:~:text=is%20in%20crisis.%22-,Watch%20how%20the%20homicide%20rate%20changes%20over%20time,-A%20Flourish%20data){watch visual}, [Chicago Mag](https://www.chicagomag.com/city-life/july-2012/austin-chicagos-deadliest-neighborhood/), and [Property Club](https://propertyclub.nyc/article/most-dangerous-neighborhoods-in-chicago#:~:text=Austin%20is%20another%20one%20of,and%2020th%20in%20property%20crime.) Austin and South Shore are at the top 10 of crime distribution relative to other community areas.
6. The general trend of crime types over the years of holiday seasons prior to, during, and post-COVID-19 shows that:
    1. The amount of incidents has decreased between 2022-2023 (it might be because the year 2023 is yet to be concluded)
    2. In most crime types, there was a steep increase in crime incidents between 2020-2021.
    3. If there wasn't a steep increase, it is likely because these crime types rely on outdoor elements, which lockdown restricted. 
#### Domestic Crime - Key Takeaways
1. Stay at home and social distancing provisions, which were imposed by the state government on 21 March 2020 led to a higher percentage of domestic related offences during the Covid period, in comparison to the pre and post Covid periods [Source](https://www.illinois.gov/news/press-release.21288.html#:~:text=The%20order%20takes%20effect%205,of%20more%20than%2010%20people.)
2. Most domestic offences occur at a residence or apartment location  i.e. private dwellings, and less so in public areas such as streets and sidewalks
3. The rate of domestic offences for residence locations has decreased from pre-Covid to post-Covid, while an opposite trend can be observed for apartment locations. This can be attributable to Covid's detrimental impact to housing affordability in Chicago driven by job losses. [Source](https://chicago.suntimes.com/2020/4/27/21238379/covid-19-affordable-housing-chicago-rent-marisa-novara-op-ed)
 Increasing trend in domestic offences in apartments from pre to post Covid may be linked to victims feeling more comfortable to seek help after the easing of government imposed restrictions following the pandemic, and due to build up of tensions in domestic relationships during the Covid period
 [Source](https://wgntv.com/news/cover-story/shadow-pandemic-of-gender-based-violence-spurs-action-in-chicago/)
#### Prolific Crimes:
1. For narcotic related offences there was a higher percentage of narcotic crimes for the pre-Covid period, in comparison to the during and post-Covid period. This can be linked to the legalisation of cannabis in Illinois, where commencing January 1, 2020 and during the pre-Covid era, adults over the age of 21 became legally able to possess, consume and purchase cannabis.
[Source](https://www.chicago.gov/city/en/sites/cannabis-information-center/home/social-consumption.html#:~:text=Pursuant%20to%20state%20law%2C%20adults,discretion%20of%20the%20property%20owner.)
2. There was a spike in motor vehicle theft for the post-Covid period. This can be attributable to the virus' impact on the supply of new cars in the motor vehicle industry due to the Covid lockdowns which caused consumer demand for new cars to surpass supply and hence creating a shortage in the supply of new cars and a spike in prices. This has also had a flow on effect on the second hand market for cars, where the supply of used vehicles cannot keep up with the demand, causing prices to increase even during the post-Covid period. As such higher car prices has made both new and second-hand cars less affordable, leading to an increase in motor vehicle theft for the post-Covid period
[Source](https://www.chicagotribune.com/coronavirus/ct-coronavirus-chicago-auto-industry-inventory-new-cars-20201002-hbxvy3qf65espn5q4zxaevs754-story.html)
[Source](https://www.chicagotribune.com/business/ct-biz-used-car-prices-20230330-chd5cfaq2jcqzk2hnqzl4fkzca-story.html)
3. Other than for narcotic and motor vehicle theft offences, Covid has not had a significant impact on how prolific a type of crime is in Chicago

#### Folder structure
``` yml
.
│   ├── Data source zips  # This folder contain ths source datasets           
│   │   ├── Datasets_1.zip                        
│   │   ├── Datasets_2.zip 
│   ├── Resources         # This folder the map boundaries of Wards, Police destricts, and community areas          
│   │   ├── Chicago_Community_Areas.svg                       
│   │   ├── Citywide Ward Map 2022.pdf
│   │   ├── Police_Districts.pdf
│   ├── holiday_seasons   # This folder include the analysis of Question 3 and the charts images
│   |   ├── Images
│   |   |   ├── offences_and_arrests.png
│   |   |   ├── offences_primary_type.png
│   |   |   ├── Top5_locations.png
│   |   |   ├── top10_community_area.png
│   |   |   ├── crime_t_holiday_seasons.png
│   ├── Geography_Analysis  # This folder include the analysis of Question 1 & 2 and the charts images
│   |   ├── .ipynb_checkpoints
│   |   |   ├── geography_analysis_1-checkpoint.ipynb
│   |   ├── Output Graphs
│   |   |   ├── 6-Month Period, Destrict 1.png
│   |   |   ├── 6-Month Period, Destrict 11.png
│   |   |   ├── 6-Month Period, Destrict 12.png
│   |   |   ├── 6-Month Period, Destrict 22.png
│   |   |   ├── 6-Month Period, Destrict 4.png
│   |   |   ├── 6-Month Period, Destrict 6.png
│   |   |   ├── 6-Month Period, Destrict 7.png
│   |   |   ├── Crime Rate, Jan - June 2019.png
│   |   |   ├── Crime Rate, Jan - June 2023.png
│   |   ├── geography_analysis_1.ipynb
│   ├── Domestic_Prolific_Crimes   # This folder contain the analysis for Question 4 & 5 as well as the charts images
│   |   ├── Domestic_Prolific_Crimes.ipynb
│   |   ├── Images
│   |   |   ├── Changes_in_Crime_Types.png
│   |   |   ├── Changes_in_Domestic.png
│   |   |   ├── Domestic_Offence_Locations.png
│   ├── filtered_1.zip     # These are the two zip files to extract & append the clean dataset. 
│   ├── filtered_2.zip
│   ├── .gitignore            
|___README.md
``` 