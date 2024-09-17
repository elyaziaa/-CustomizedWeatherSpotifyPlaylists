# Assignment 1: Customized Spotify Playlists Based on Current Weather at a US State
By:Elyazia Abbas and Aysa Binte Masud

# Description of Program & Purpose: 

Our program uses two APIs, the Spotify API, and the weather io API, in order to ask the user to type in a state in the US, and receive a customized Spotify playlist of songs to listen to under the genre that matches best with the current weather at that State. A fun purpose of this project is a fun way to be able to give playlist recommendations to friends or family that live in other states, even if you do not experience the same weather as them! 


# APIs Used: Tomorrow IO & Spotify

# Tomorrow IO:
First we used the Tomorrow API, which is a weather API. It takes in longitude and latitude as required parameters, and a few other optional parameters that we did not use. For that reason, we had to limit our user to input only states in the United States, and we used a dictionary to match all the states and their respective longitude and latitudes. We chose this API mainly because its also in json format, which we are familiar with. ALso, we experimented with it a few times, and the weather was always accurate, as we would compare it to the weather app on our phones. 

# Spotify:
We obtained song recommendations based on the weather category by utilizing the Spotify API. There are multiple APIs available via the Spotify API to retrieve information on songs, playlists, and recommendations. We worked on the recommendations endpoint in particular for our use case since it makes track recommendations based on seed genres.We had to authenticate using client credentials, which are made up of a client_id and client_secret, in order to access the Spotify API. We acquired these credentials after registering our app on Spotify for Developers. The spotipy library from Spotify made interacting with the API and managing the permission procedure simple.
We picked the Spotify API because of its extensive library of music information and adaptable recommendation system. In our code, we implemented map weather categories (like chilly, warm) to particular genres (like chill, party). This made it possible for us to play music that reflects the attitude of the current weather. Because it allows us to input genres as seeds and returns a carefully selected list of songs, the recommendations endpoint was especially helpful for achieving our objective of providing weather-based music suggestions.Overall, we tested a range of endpoints and discovered that the recommended outcomes were consistently appropriate offering a pleasant and weather-dependent experience.



# Instructions on how to use the feature:

1- Make sure to put secretes names and values in the secretes section of the collab notebook 
2-Make sure to give the notebook Access to the secrets page, you should see three keys, the weather key, client secrete, and client id.
3- Run All Cells on the Notebook.
4- The last cell will ask you to input a US state, input the State, and the playlist will be displayed.


