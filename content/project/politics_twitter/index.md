---
title: An Interactive Visualization of Twitter's Sentiment to President Biden's State of the Union (CSE 512 Final Project)
summary: To gain insight into how Americans feel about current domestic and foreign policies, we performed sentiment analysis of tweets about the 2022 State of the Union (SOTU) and created an interactive visualization of the results on an Albers projection of North America.

tags:
- Data Visualization
- Software Engineering
- Natural language processing
- Sentiment analysis

date: "2022-05-25T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption:
  focal_point:

links:
- icon: github
  icon_pack: fab
  name: Github Site
  url: https://brian-cy-chang.github.io/CSE512_spr2022/
url_code: "https://github.com/brian-cy-chang/CSE512_spr2022"
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides:
---

The project deliverable was an interactive visualization of sentiment analysis with respect to Tweets related to President Biden's 2022 State of the Union. The visualization is built on [D3]. This project was completed in collaboration with Dr. Richard Green.

<!-- ##### Included in the dashboard:
- Maps and complementary histograms of month-specific data pertaining to:
    -  Number of deaths per county; 
    -  Number of positive case counts per county; 
    -  Population density per county (based on 2010 US Census estimates). -->
<!-- 
Below is the screenshot for comparison view dashboard. Note that users can hover their mouse on different counties to see details as shown in the screenshot.
<br/>
<br/>
<img src="CO-MAP-V_screenshot_1.png" width="75%">
<br/>
<br/>
Below is another screenshot for single view dashboard:
<br/>
<br/>
<img src="CO-MAP-V_screenshot_2.png" width="75%">
<br/>
<br/> -->

## Background
This project focused on various data visualization techniques, namely creating an interactive map and data points. The motivation behind the project is as follows.

There has been growing political division between Democrats and Republicans, the two major political parties in the United States, the past decade. At a time in which Republicans are pushing to overturn Roe V. Wade, block gun control, and continue gerrymandering, it is paramount that Democrats and President Biden earn votes on the campaign trail leading into the 2022 mid-term elections and the 2024 presidential election. To gain insight into how Americans feel about current domestic and foreign policies, we performed sentiment analysis of tweets about the 2022 State of the Union (SOTU). As the SOTU covered many topics, such as sanctioning Russia, rising inflation, the COVID-19 pandemic, and the American Rescue Plan, we believe it is a good proxy for important domestic and foreign policies. 

### Goals:
- Query data using Twitter's API and perform data cleaning.
- With the cleaned data, perform sentiment analysis using an open source transformer model from [HuggingFace].
- Create an interactive visualization that allows both desktop and mobile users to see the respective Tweet sentiments on a map of North America built on [D3].

<!-- # Technical Information

### Installation and set up

First, make sure that you have Python via Anaconda installed, [https://conda.pydata.org/miniconda.html](https://conda.pydata.org/miniconda.html). 

Use the YML environment file to create an identical environment on your local or remote machine:
    
    conda create --name myenv —environment.yml

For reference: [This is our YML for our conda virtual environment]; and [this is the requirements.txt file]. -->
<!-- 

# Tips for Modifying CO-MAP-V Code for Personal Use
First, clone our repository.
    
    git clone https://github.com/co-map-v/co-map-v.github.io

Then make the following changes as needed. -->

## Data
Our dataset includes Tweets with a mention of `#SOTU`, `#StateoftheUnion`, or `"Biden"`, between 2022-03-01 00:00:00 to 2022-03-07 11:59:59. Queried tweets could not be retweets, must have a corresponding geotag, and written in English.
To create the map of North America, we used a GeoJSON file of the US state boundaries. You can see our visualization by clicking [here](https://brian-cy-chang.github.io/CSE512_spr2022/).

### Twitter Data
Please refer to the official Twitter [API] to query Tweets.

### GeoJson Data
* Get the GeoJSON files from https://github.com/brian-cy-chang/CSE512_spr2022.

<!-- ### Population Data
* Get the needed census data of population by county from https://data.census.gov.
* Name the file 'population2010.csv', replace our ~/comapv/data/population2010.csv with your own file and ensure it is formatted the same way (e.g. same columns and data types).
### Patient Data
* If using data formatted in the OMOP CDM (v5.3.1), refer to the first few commented lines of ~/comapv/data/data_cleaning.py which includes the SQL script used for data extraction from the synthea data formatted in the OMOP CDM:

   ```SQL
   SELECT DISTINCT l.zip, l.county, p.person_id, p.gender_source_value,
   p.birth_datetime, p.death_datetime, p.race_source_value,
   p.ethnicity_source_value, c.condition_start_datetime,
   c.condition_concept_id
   FROM person p
   INNER JOIN condition_occurrence c ON c.person_id = p.person_id
   INNER JOIN location l on l.location_id = p.location_id
   WHERE condition_concept_id = '37311061' --Disease caused by 2019-nCoV
   ```

* If not using data formatted in the OMOP CDM, make sure to query your data with the result formatted the same (e.g. same columns and data types) as the data are in ~/comapv/data/data-1605136079581.csv and name your file 'data-1605136079581.csv' for ease of use to ensure you won't have to rename the file when it is referenced in analysis and/or testing. -->

### Data Cleaning
<!-- 1. Make sure your data ('data-1605136079581.csv' and 'population2010.csv') are formatted the same as they are in this repository.
2. Edit ~/comapv/data/data_clean.py to change the name of the output file (currently 'covid_ma_positive_death_counts.csv') to a name suitable for your project.
3. Run ~/comapv/data/data_clean.py.
4. Adjust tests as needed if name of output file ('covid_ma_positive_death_counts.csv') has changed. -->
Please clean and format your data following the format at https://github.com/brian-cy-chang/CSE512_spr2022/blob/main/df_all.csv.
These will include the sentiment analysis scores from the [HuggingFace] model.
<!-- 
## Web deployment
* Refer to the documentation seen here regarding heroku and dash: 
   * https://dash.plotly.com/deployment 
   * https://devcenter.heroku.com/articles/github-integration -->


[//]: # (Reference Links)

   [Plotly]: <https://www.plotly.com/>
   [Dash]: <https://dash.plotly.com/>
   [OHDSI]: <https://forums.ohdsi.org/t/synthetic-data-with-simulated-covid-outbreak/10256>
   [TopoJSON Github Repository]: <https://www.github.com/deldersveld/topojson/tree/master/countries/us-states>
   [Heroku]: <https://www.heroku.com>
   [Functional]: <https://github.com/co-map-v/co-map-v.github.io/blob/main/docs/Functional%20Specification.pdf>
   [Component]: <https://github.com/co-map-v/co-map-v.github.io/blob/main/docs/Component%20Specification.pdf>
   [This is our YML for our conda virtual environment]: <https://github.com/co-map-v/co-map-v.github.io/blob/main/environment.yml>
   [this is the requirements.txt file]: <https://github.com/co-map-v/co-map-v.github.io/blob/main/requirements.txt>
   [D3]: <https://d3js.org/>
   [HuggingFace]: <https://huggingface.co/>
   [API]: <https://developer.twitter.com/apitools/>