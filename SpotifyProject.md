Spotify Project


PROJECT OVERVIEW


This data analysis project provides insights about the music performance focusing on the top artists,albums,and songs that contributed to the multiple streams that occurred during 2018 and 2019. These insights can be used to make recommendations towards marketing strategies that can be implemented to further on increase the number of streamers on their platform.
The data was a spotify songs excel workbook file. It included information about different songs, with the artists from each song starting from 1905. 
I focused on displaying visualisations for 2018 and 2019(which I filtered) with the following visuals:

Summary Report

Total Albums Released

Top 5 Played Artists

Top 5 Songs(Overall) 

Top 5 Albums(Overall) with their respective artists. 

STEPS FOLLOWED
1. Loaded the data into PowerBI.
2. I did not have to do any data cleaning as they were no errors,formatting issues,duplicates,nulls, or empty rows.
3. Created a new Date Column:
   
 3.1. I created a new table called Calendar
 
 3.2. Copied the date column from the spotify_songs table and pasted it in the Calendar table
 
 3.3. Then I created a calculated column to showcase the dates from the first day of the month to the last day of 
   the month because the dates were not in order.
   
   Snapshot of Calculated Column:


   
  ![Calendar](https://github.com/khelz424/Spotify-Project/assets/141655852/81dac18d-0e7b-4e4d-82f4-727fa0c8e522)

4. Merged queries to create a new id column for the track_album_name:


  STEPS FOLLOWED

  
   4.1. Firstly created a table called Albums.


   4.2. Copied the track_album_name column.


   4.3. Clicked on add column and then clicked on index column starting from 1.
  
  
   4.4. Clicked on merge query to merge the spotify_songs and Albums table based off the track_album_name column as 
       it is a common column in both tables.


   4.5. In the spotify_songs table I expanded the Albums column and only selected the track_album_name_new_id 
       column to be displayed.


     Snapshot:


![Screenshot (24)](https://github.com/khelz424/Spotify-Project/assets/141655852/03220659-d0d9-4bb5-a8ad-eba57c7e53ad)


VISUAL 1: Summary Report

This visual provides an overview about the top 5 played artists,total albums released, and the top 5 albums.


![Screenshot (41)](https://github.com/user-attachments/assets/127c331f-dbf6-43c0-9ee8-181c69178565)




The visuals beyond this point are reports that provide further information if a user is interested in a specific visuals.

VISUAL 2: Total Albums Per Genre


This visual provides information about the the total albums released in 2018 and 2019 based off the following genres represented in the diagram. 

![Screenshot (42)](https://github.com/user-attachments/assets/55a6b1cf-fbd6-4d5a-8323-705fc449b18a)





I decided to go with a Donut Chart which has Total Albums under the Values field and added the Date column calculated under the Legend field, which I filtered to display the year of 2018 and 2019.
In order to create Total Albums as a value I created a measure which is the sum of the track_album_name_new_id column that was merged into the spotify_songs table(as previously mentioned).

Snapshot of Total Albums Measure created:


![Screenshot (4)](https://github.com/khelz424/Spotify-Project/assets/141655852/7946c674-501a-4215-9e13-44b5b08e37d9)



Lastly I included a slicer that provides information about the different genres,which will enable a user to view the total albums released for a particular genre they are interested in.


Overall,this visual provides Spotify with information that will help them to understand the number of albums released in 2018 and 2019 based off each genre to get a better uderstanding of the market.

VISUAL 3: Top 5 Played Artists Analysis


This visual provides information about the top 5 artists that were the most played based off the following genres.

![Screenshot (44)](https://github.com/user-attachments/assets/a5ab2de8-e49a-492b-a0fa-ef079cff9de4)


The visual is displayed as a clustered column chart with the Y-axis being the popularity figures and the X-axis being the year. 
In order to have the top 5 artists displayed on the visual I created a filter for the Artist column which shows the top 5 artists based off the sum of the track popularity. 

Snapshot Of Filter:


![Screenshot (11)](https://github.com/khelz424/Spotify-Project/assets/141655852/47e11727-3e03-4acc-9af1-186f3c36434e)

Lastly,  I included a slicer which will allow a user to pick the genre that they are the most interested in.


Overall,this visual can help users to identify which artists based off the different genres were listened to the most. Hence understanding the users' tastes and which musicians contribute to the streaming success of Spotify.

VISUAL 5: Top 5 Albums Analysis(Overall)


This visual provides information about the top 5 albums listened to based off the top 5 artists and their popularity.

![Screenshot (43)](https://github.com/user-attachments/assets/52838dff-cad1-4141-8948-99bdcecb9e12)


I filtered the visual based off popularity, track_artist, and lastly by the Album. The Album was filtered by the top 5 albums by popularity.

Snapshot Of Filter:


![Screenshot (17)](https://github.com/khelz424/Spotify-Project/assets/141655852/78cad3e8-7ae3-44b7-83f2-cbaa28f58014)


I included a slicer which showcases the year. It will allow a user to visualise the top 5 albums based off the top 5 artists between 2018 and 2019. Based off what they are interested in.


Overall, this visual will provide information about the top 5 artists and their respective albums that had the most popularity as well as the total sum of the popularity.


CONCLUSION

In conclusion, through the use of PowerBI, this project has explored the data to facilitate in the creation of visuals which will be used by the users to extract insights to facilitate in making informative decisions about their approach to maximise their future performance in the music industry.
