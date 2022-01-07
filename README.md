# YouTube-Statistics-for-trending-videos
YouTube should consider these statistics to understand what are the major factors which are involved for the video to be in trending status. YouTube has given multiple factors being responsible for the video to be trending status and we can narrow the filter to minimal categories which would help the video/content creators to ensure that their video is being reached out to wide audience.
**Description of Data:**
Data Source: 
URL: https://www.kaggle.com/datasnaek/youtube-new
Format: csv
Data Description Report:
The dataset used for the analysis consists of trending videos from 2017-2018 which are for United States region. The dataset constitutes of 40950 rows and 16 columns. 

**Data Preparation Report:**
Creating new attributes:
o	Modified published_time and removed 000Z by using delimited function on excel. 
o	Created additional column named as published_time

**Clean Missing Data:**
We are using Azure ML Studio for data cleaning and preparation:

![image](https://user-images.githubusercontent.com/97264434/148621151-cf573d7b-b268-443b-be88-8c30f93c7f2b.png)
 
Reason for missing data: MCAR: Missing completely at random. We are using imputation method ‘MICE’ to fill the missing values with number of iterations being 5. We are generating the missing value indicator column to identify the output results of Missing values.
Once the values are imputed, we do not see any missing values:

![image](https://user-images.githubusercontent.com/97264434/148621194-7ce3e0fb-691f-42ea-9787-1b758cad7020.png)

**Data Transformation**
We have transformed the data using apply math pill by using the function Ln+1 to reduce the skewness.
![image](https://user-images.githubusercontent.com/97264434/148621224-5f734337-5086-4791-900d-eb6c74fbbe12.png)

 
