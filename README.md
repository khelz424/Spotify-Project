1. Spotify Project

DASHBOARD LINK: https://nicotechnologiesmw-my.sharepoint.com/:u:/g/personal/nohakhelha_chanje_nicotechnologies_com/EZ_CrI--kxRNuGowhIW828UByvHPn5SGfEDM4IOPXAidMA?e=UrgxLX

STATEMENT

The data was a spotify songs excel workbook file. It included information about different songs, with the artists from each song starting from 1905. 
I focused on displaying visualisations about the Total Albums Released per Genre, Top 5 Played Artists per Genre, Top 5 songs per the top 3 artists overall, 
and the Top 5 Albums overall ith their respective artists. I filtered the analysis to only present information for 2018 and 2019 for each visual.

STEPS FOLLOWED
1. Loaded the data into PowerBI
2. I did not have to do any data cleaning as they were no errors,duplicates,nulls, or empty rows
3. Created a Calculated column for the date
   3.1. created a new table called Calendar
   3.2. Copied the date column and pasted it in the Calendar table
   3.3. Then I created a calculated column to showcase the dates from the first day of the month to the last day at the moment the dates were not in order
   
   Snapshot of Calculated Column:

   
  ![Calendar](https://github.com/khelz424/Spotify-Project/assets/141655852/81dac18d-0e7b-4e4d-82f4-727fa0c8e522)


  4. Merged queries to create a new id column for the track_album_name
     4.1. Created a table called Albums
     4.2. Copied the track_album_name column
     4.3. Clicked on add column and then clicked on index column starting from 1
     4.4. Clicked on merge query to merge the spotify_songs and Albums table based off the track_album_name column as it is a common column in both tables
     4.5. In the spotify_songs table I expanded the Albums column and only selected the track_album_name_new_id column to be displayed

     Snapshot:


     ![Screenshot (2)](https://github.com/khelz424/Spotify-Project/assets/141655852/57258754-ee5a-41be-bb28-24ef1229b228)




