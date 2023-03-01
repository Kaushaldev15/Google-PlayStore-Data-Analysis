<h1 align='center'>Google PlayStore Data Analysis<h1>
<p align="center">
    <img width="500" src="images/logo.gif" alt="logo">
  <h3 align='center'>Project by - Kaushal Devlekar and Suhita Vaidya<h3>
</p>
    
<h2>• Objective</h2>
<p>
  The objective of this project is to gain insights into the applications hosted on Google Playstore and the sentiment of their user reviews and present these ingsights in the form of visualisation which can be used to improve the overall experience and optimise the application development processes.
</p>
    

<h2>• Tools Used</h2>
<p>
  > Microsoft Excel <br>
  > Google Colab (Python libraries - Numpy, Pandas, Seaborn, Matplotlib, TextBlob)<br>
  > MySQL Workbench <br>
  >PowerBI
</p>    

<h2>• Project Files Description</h2>
<p>
This Project includes 1 colab notebook, 1 SQL text file and 1 PowerBI report pdf :
  
<b>Google Colab - </b>Includes all the code and their outputs executed in the python environment.
  
<b>MySQL - </b>Includes all the queries that answer the problem statements based on the dataset.
  
<b>Power BI - </b>https://app.powerbi.com/view?r=eyJrIjoiODMwYzNkN2ItYmZhZi00MjNmLTg4YTMtNDM3ZWZmNTRlMzg2IiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9 (Please refer to PowerBI Reports.pdf for python visualisations)
  
  
<b>Data Source : </b> Kaggle <br>
<b>playstore_apps.csv - <b/>It contains the basic details of the app like number of user reviews, ratings, etc. <br>
- App: It contains the name of the app with a short description (optional).
- Category: This section gives the category to which an app belongs. In this dataset, the apps are divided among 33 categories.
- Size: The disk space required to install the respective app.
- Rating: The average rating given by the users for the respective app. It can be in between 1 and 5.
- Reviews: The number of users that have dropped a review for the respective app.
- Installs: The approximate number of times the respective app was installed.
- Type: It states whether an app is free to use or paid.
- Price: It gives the price payable to install the app. For free type apps, the price is zero.
- Content rating: It states which age group is suitable to consume the content of the respective app.
- Genres: It gives the genre(s) to which the respective app belongs.
- Last updated: It gives the day in which the latest update for the respective app was released.
- Current Ver: It gives the current version of the respective app.
- Android Ver: It gives the android version of the respective app.<br>
    
    
<b>playstore_reviews.csv - <b/>It contains the user reviews for respective app.<br>
- App: It contains the name of the app with a short description (optional).
- Translated_Review: It contains the English translation of the review dropped by the user of the app.<br>
    

</p>    
    
<h2>• Steps Involved</h2>
<p>
      <h3>Data Cleaning and Transforming</h3><br>
    To prepare the data for analysis, we performed several data cleaning steps. First, we checked for null values to ensure that there were no missing pieces of data. We also identified and removed outliers, especially in cases where ratings had a specific range. If null values existed, we inserted values using the modeValue method. We modified data values, for size column we removed symbols like K and M and replaced them with their respective values, as well as removed unwanted characters like "+" and ",". We changed data types of columns to ensure that the data was in a format that was easy to analyze. Finally, we dropped duplicates and checked unique values to ensure the integrity of the data and that it was compliant with the intended datatype. A new column 'Revenue' was added by multiplying the prices and installs value for each record.
      <h3>Natural Langugage Processing</h3><br>
      • This project performs sentiment analysis on Google Play Store reviews using NLP and TextBlob. <br>
      • The analysis is based on three metrics: polarity, subjectivity, and sentiment.<br>
      • The polarity column indicates the sentiment of each review as positive, negative, or neutral.<br>
      • The subjectivity column measures the degree of personal opinion in the review on a scale of 0 to 1, where 0 represents a factual statement and 1 represents a highly opinionated statement.<br>
      • The sentiment column is an aggregate score between -1 and 1 that takes into account both polarity and subjectivity.<br>
      • A score of -1 indicates an extremely negative review, 1 indicates an extremely positive review, and 0 indicates a neutral review.<br>
      • These insights can be useful for improving product quality and customer satisfaction.<br>
      <h3>Exploratory Data Analysis</h3><br>
</p>
      
<h2>• Problem Statement</h2>
<p>
  1. Total number of apps present in the Google playstore dataset. <br>
  2. Number of Categories present in the dataset.<br>
  3. All categories with the number of apps in them.<br>
  4. Average rating and average size of all the apps.<br>
  5. Overview of all categories wrt Number of installs, least rated app, highest rated app, number of free apps and number of paid apps in that category in that category.<br>
  6. Which are the top 10 highest rated apps in the given available dataset?<br>
  7. What are the number of installs and reviews for the above apps? Return the apps with the highest reviews to the top.<br>
  8. Which app has the highest number of reviews? Also, mention the number of reviews and category of the app.<br>
  9. What is the total amount of revenue generated by the google play store by hosting apps? (Whenever a user buys apps  from the google play store, the amount is considered in the revenue)<br>
  10. Which Category of google play store apps has the highest number of installs? Also, find out the total number of installs for that particular category.<br>
  11. Which Genre has the most number of published apps?<br>
  12. Find the count of apps in each content rating based on App type.<br>
  13. Create a new column to bucket rating to high(4-5), medium(2-4), low(0-2). Return the app names.<br>
  14. Return categories with their sentiment counts for each type of sentiment.<br>
  15. Provide the list of all games ordered in such a way that the game that has the highest number of installs is displayed on the top.<br>
  16. List all non-entertainment and non-education apps that are rated by everyone or teen.<br>
  17. List all the apps whose app names contain the letter “i” or start with the letter “D”<br>
  18. Return the app names, categories, sizes, release dates (rename it to “Last Updated”) of apps whose app names have more than 1 word, and whose categories are music and social, and whose sizes are bigger than 10. Order the output result by maximum installs in descending order, then release dates in ascending order.<br>
  19. Find the number of apps in each category that have a rating greater than the average rating.<br>
  20. List the largest app size within each app category.<br>
</p>
      
<h2>• Challenges Faced</h2>
<p>
  
</p>      
      
<h2>• Conclusion</h2>
<p>
  
</p>      
