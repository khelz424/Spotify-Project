Spotify Project


PROJECT OVERVIEW



This data analysis project provides insights about the music performance focusing on the top artists,albums,and songs that contributed to the multiple streams that occurred during 2018 and 2019. These insights can be used to make recommendations towards marketing strategies that can be implemented to further on increase the number of streamers on their platform.
The data was a spotify songs excel workbook file. It included information about different songs, with the artists from each song starting from 1905. 
I focused on displaying visualisations for 2018 and 2019(which I filtered) with the following visuals:

Total Albums Released

Top 5 Played Artists

Top 5 Songs(Overall) 

Top 5 Albums(Overall) with their respective artists. 

STEPS FOLLOWED
1. Loaded the data into PowerBI
2. I did not have to do any data cleaning as they were no errors,formatting issues,duplicates,nulls, or empty rows
3. Created a Calculated column for the date. Firslty; I created a new table called Calendar,copied the date column and pasted it in the Calendar table, and then I created a calculated column to showcase the dates from the first day of the month to the last day of the month because the dates were not in order.
   
   Snapshot of Calculated Column:


   
  ![Calendar](https://github.com/khelz424/Spotify-Project/assets/141655852/81dac18d-0e7b-4e4d-82f4-727fa0c8e522)


  4. Merged queries to create a new id column for the track_album_name.
     I firstly created a table called Albums.Secondly;copied the track_album_name column.Thirdly;clicked on add column and then clicked on index column starting from 1.Furthermore;clicked on merge query to merge the spotify_songs and Albums table based off the track_album_name column as it is a common column in both tables.
     Lastly;in the spotify_songs table I expanded the Albums column and only selected the track_album_name_new_id column to be displayed.


     Snapshot:

     ![Screenshot (2)](https://github.com/khelz424/Spotify-Project/assets/141655852/57258754-ee5a-41be-bb28-24ef1229b228)




VISUAL 1: Total Albums Per Genre
This visual provides information about the the total albums released in 2018 and 2019 based off the following genres represented in the diagram. 


![Screenshot (3)](https://github.com/khelz424/Spotify-Project/assets/141655852/a591b258-07b9-466b-a227-fc6d27ee22c0)



I decided to go with a Donut Chart which has Total Albums under the Values field and added the Date column calculated under the Legend field, which I filtered to display the year of 2018 and 2019.
In order to create Total Albums as a value I created a measure which is the sum of the track_album_name_new_id column that was merged into the spotify_songs table(as previously mentioned).

Snapshot of Total Albums Measure created:


![Screenshot (4)](https://github.com/khelz424/Spotify-Project/assets/141655852/7946c674-501a-4215-9e13-44b5b08e37d9)



Lastly I included a slicer that provides information about the different genres,which will enable a user to view the total albums released for a particular genre they are interested in.


VISUAL 2: Top 5 Played Artists Analysis
This visual provides information about the top 5 artists that were the most played based off the following genres.

![Screenshot (7)](https://github.com/khelz424/Spotify-Project/assets/141655852/8a52e04c-be89-4f4c-ab94-97edee7b3d86)

The visual is displayed as a clustered column chart with the Y-axis being the popularity figures and the X-axis being the year. 
In order to have the top 5 artists displayed on the visual I created a filter for the Artist column which shows the top 5 artists based off the sum of the track popularity. 

Snapshot Of Filter:


![Screenshot (11)](https://github.com/khelz424/Spotify-Project/assets/141655852/47e11727-3e03-4acc-9af1-186f3c36434e)

This can help users to identify which artists based off the different genres were listened to the most. Hence understanding the users' tastes and which musicians contribute to the streaming success of Spotify.

VISUAL 3: Top 5 Songs Analysis(Overall)
This visual provides information about the top 5 songs listened to based off the top 3 artists regardless of genre.

![Screenshot (9)](https://github.com/khelz424/Spotify-Project/assets/141655852/cfa81f25-3c95-4858-aa78-7d3436de4795)

The visuals are represented using a multi-row card as it will display the name of the artist and their top 5 songs.
I filtered each card by the Artist and the Track name by the top 5 songs based off the sum of the track popularity 

Snapshot Of Filter:

![Screenshot (10)](https://github.com/khelz424/Spotify-Project/assets/141655852/eac9ec27-9513-4ed7-9bed-47f0baf24d89)




VISUAL 4: Top 5 Albums Analysis(Overall)
This visual provides information about the top 5 albums listened to based off the top 5 artists and their popularity.

![Screenshot (12)](https://github.com/khelz424/Spotify-Project/assets/141655852/41983a63-1253-47fe-a48c-35ce0d1617de)

I filtered the visual based off popularity, track_artist, and lastly by the Album. The Album was filtered by the top 5 albums by popularity.

Snapshot Of Filter:


![Screenshot (17)](https://github.com/khelz424/Spotify-Project/assets/141655852/78cad3e8-7ae3-44b7-83f2-cbaa28f58014)



