# Crime Analysis

### Project description:
This is a group project that included a creation of a workflow in GitHub to collaborate on an observetional study of crime in the city of Chicago, Illinois. The purpose of the analysis and the main reaseach question was **"how did COVID-19 impact crime in Chicago?"** To conclude on this question, the following sub-questions were analysed: 
1. Did covid impact the distribution of crime in Chicago?
2. Did covid impacted the crime types?
3. Has covid had an impact during holiday seasons?
4. Has it impacted the number of domestic crime?

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


#### TLDR - Conclusions
**Crime Destribution - Key Takeaways**
1. 
**Crime Types - Key Takeaways**
1. 
**Holiday Seasons - Key Takeaways**
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
**Domestic Crime - Key Takeaways**
1. 

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
│   ├── Geography_Analysis  # This folder include the analysis of Question 1 & 4 and the charts images
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
│   ├── filtered_1.zip     # These are the two zip files to extract & append the clean dataset. 
│   ├── filtered_2.zip
│   ├── .gitignore            
|___README.md
``` 