# DataViz
## CS226 Project Proposal (Group Name: Data VIZards)
**Visualization of geospatial data for drought, vegetation, temperature, and wildfire**

       	 Mrunali Lachake              Kaushik Daiv                Dhananjay Gavade              Shivanshu Gupta                     
            Computer Science                Computer Science                   Computer Science                        Computer Science 
            UCR SID - 862394872          UCR SID - 862393181            UCR SID - 862395404                 UCR SID - 862393340
          	mlach008@ucr.edu                kdaiv001@ucr.edu                   dgava001@ucr.edu                       sgupt103@ucr.ed



**BACKGROUND & MOTIVATION**
A major problem in California is the prevalence of droughts and wildfires. Over the past few years, California's drought circumstances have changed drastically. Lack of water causes droughts and the same is true for wildfires. These events can be associated with temperature because when the latter rises, water availability decreases, which may in turn cause droughts and wildfires as well as impact vegetation. Therefore, we wish to visualize the correlation between drought, vegetation, temperature, and wildfire in California.
We propose a visualization tool that can be used to find the correlation between drought, vegetation, temperature, and wildfire. Users can analyze the effect of one on the other to gain insights such as a) Does temperature affect the drought?, b) How increasing temperature affects the wildfire?, c) How does vegetation pattern change according to drought conditions?
We will discuss the dataset, project outcome, evaluation, and milestones in further sections.

**DATASET DESCRIPTION**
We will utilize the satellite data of vegetation and drought provided by the United States Geological Survey[2][4]. Furthermore, we plan to study the effects of temperature on drought and wildfire. To achieve this, we are using a temperature dataset from kaggle[3] and a wildfire dataset from WildfireDB[1].
1 Drought Dataset
When we look at drought data, we have considered two main factors - streamflow and groundwater level in a certain area. 
The dataset contains tabular data for different sites identified by individual site id, site name, latitude/longitude, and the amount of water (feet for groundwater and cubic feet/second for stream). Data is recorded every 15 minutes.

2 Temperature Dataset
The temperature dataset is in tabular format and includes attributes like latitude, longitude, city, date, and average temperature for a month. The dataset includes 1977 records.

3 Wildfire Dataset
This dataset consists of spatial polygons of wildfire zones along with some additional features like minimum/maximum temperature, fire radiative power(FRP), and fire acquisition time[1]. 

4 Vegetation Dataset
The vegetation Landsat dataset comprises Tiff-formatted satellite images along with location-specific metadata. The dataset is about 3GB in size and consists of 1236 satellite photos for Riverside County.

We are examining data of Riverside county for the past 20 years in our prototype because of resource limitations.


**OUTCOME**

We make use of geospatial information on the weather, vegetation, wildfires, and level of drought in Riverside County, California. With data gathered over a 20-year period, our project combines big-data methodologies for data visualization. Users will be able to choose multiple parameters while viewing satellite data for all 4 categories in order to gain insights and find correlations across the area.

**RELEVANCE TO BIG DATA**

In this project, we will be using 4 different datasets viz, temperature, wildfire, drought, and vegetation. Our data corresponds to the 3 V’s of Big Data characteristics as follows:
Volume: The size of the data is enormous given that we are utilizing 4 datasets which consist of a batch, image, and geographical data. To process this data, we must leverage big data technologies like Spark and Hadoop.
Variety: Our datasets contain a variety of data including image, spatial, temporal, numerical, etc. To handle this, we will normalize and transform the data.
Veracity: As we are using datasets from different sources we will preprocess the data to make it consistent, consolidated, and accurate.

**EVALUATION**

We are going to evaluate our tool with two different approaches. First, we will evaluate if there is any correlation between the four datasets. We will be using different correlation techniques such as Spearman to analyze and evaluate the relationship. Other than correlation we will evaluate the accuracy of spatial data of vegetation, temperature, drought, and wildfire with K-means clustering. 

**MILESTONES**

Project requirement gathering and Environment setup - 10/22/2022
Setup storage and load data - 10/25/2022
Preprocess datasets - 11/05/2022
Transform dataset and design data pipeline - 11/11/2022
Design and develop visualization report - 11/18/2022
Create presentation - 11/23//2022

**REFERENCES**
[1]	Samriddhi Singla, Ayan Mukhopadhyay, Michael Wilbur, Tina Diao, Vinayak Gajjewar, Ahmed Eldawy, Mykel Kochenderfer, Ross Shachter, and Abhishek Dubey, 2021. WildfireDB: An Open-Source Dataset Connecting Wildfire Spread with Relevant Determinants, In the 35th Conference on Neural Information Processing Systems (NeurIPS 2021).
[2]	https://ca.water.usgs.gov/california-drought/california-drought-resources.html
[3]	https://www.kaggle.com/code/theroffness/california-temperature/data
[4]	https://earthexplorer.usgs.gov/
