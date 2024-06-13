1. Spotify Project

DASHBOARD LINK: https://nicotechnologiesmw-my.sharepoint.com/:u:/g/personal/nohakhelha_chanje_nicotechnologies_com/EZ_CrI--kxRNuGowhIW828UByvHPn5SGfEDM4IOPXAidMA?e=UrgxLX

STATEMENT

The data was a spotify songs excel workbook file. It included information about different songs, with the artists from each song starting from 1905. 
I focused on displaying visualisations about the Total Albums Released per Genre, Top 5 Played Artists per Genre, Top 5 songs per the top 3 artists overall, 
and the Top 5 Albums overall ith their respective artists. I filtered the analysis to only present information for 2018 and 2019 for each visual.

STEPS FOLLOWED
1. Loaded the data into PowerBI
2. I did not have to do any data cleaning as they were no errors,duplicates,nulls, or empty rows
3. Created a Calculated column for the date. Firslty; I created a new table called Calendar,copied the date column and pasted it in the Calendar table, and then I created a calculated column to showcase the dates from the first day of the month to the last day of the month because the dates were not in order.
   
   Snapshot of Calculated Column:

   
  ![Calendar](https://github.com/khelz424/Spotify-Project/assets/141655852/81dac18d-0e7b-4e4d-82f4-727fa0c8e522)


  4. Merged queries to create a new id column for the track_album_name. I firstly created a table called Albums, secondly;copied the track_album_name column, thirdly; clicked on add column and then clicked on index column starting from 1, furthermore; clicked on merge query to merge the spotify_songs and Albums table based off the track_album_name column as it is a common column in both tables, lastly; in the spotify_songs table I expanded the Albums column and only selected the track_album_name_new_id column to be displayed.

     Snapshot:


     ![Screenshot (2)](https://github.com/khelz424/Spotify-Project/assets/141655852/57258754-ee5a-41be-bb28-24ef1229b228)


VISUAL 1: Total Albums Per Genre
This visual provides information about the the total albums released in 2018 and 2019 based off the following genres represented in the diagram. 

![Screenshot (3)](https://github.com/khelz424/Spotify-Project/assets/141655852/a591b258-07b9-466b-a227-fc6d27ee22c0)



I decided to go with a Donut Chart which has Total Albums under the Values field and added the Date column calculated under the Legend field, which I filtered to display the year of 2018 and 2019.
In order to create Total Albums as a value I created a measure which is the sum of the track_album_name_new_id column that was merged into the spotify_songs table(as previously mentioned).

Snapshot of Total Albums Measure created:
![Screenshot (4)](https://github.com/khelz424/Spotify-Project/assets/141655852/7946c674-501a-4215-9e13-44b5b08e37d9)



Lastly I included a slicer that provides information about the different genres,which will enable a user to view the total albums released for a particular genre they are interested in based off 2018 and 2019.


VISUAL 2: Top 5 played artists analysis
This visual provides information about th top 5 artists that were the most played in 2018 and 2019 based off the following genres.

![Screenshot (7)](https://github.com/khelz424/Spotify-Project/assets/141655852/8a52e04c-be89-4f4c-ab94-97edee7b3d86)





