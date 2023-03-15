# Spotify-Recommender

  As a musician, I cannot let pass a day without opening the Spotify app and play some music according my mood. That made me to wonder why I haven't considered using my own data collection along (how many?) years to, first, make a small exploratory analysis and second, try to develop a classification model that would predict whether I liked a song or not.

In order to achieve my goal, I started to look into previous pieces of work which have been already done in the community of Data Scientists (each of them will be enumerated at the end), and I discovered that Spotify already has an API that allows us to extract what they named the “Audio-Features”, which are a certain kind of attributes that belongs to each song. Some of them are very subjective fields, for instance, how danceable a song is or how much energy a song can give you, and others more objective like Tempo, Key or Mode (minor or major).

Gladly, it exists a Python Library called Spotipy, which lets us connect to the API in an easy and quick way. It's worth mentioning that a Spotify "Dev Account" will be required, but its process is easy and free of charge.

  
 ## Enviroment
 
The whole analysis was created in a Google Colab Jupyter Notebook with each of the following tools:
 
- A **Dev Account** in Spotify
- **Spotipy** Library for getting our data
-	**Plotly** Library for an interactive data visualization
-	**Pandas** and **Numpy** Library for data analysis
-	**Scikit-Learn** Library for our Machine Learning model

## EDA
  
 We created 2 lists: One based on all the songs that I have liked along the years (df_SI), and other one based on all the genres that I do not like such as Reggaeton and Cumbia 420 (df_NO). Each of them has approx. 400 songs, and below are some facts about their features.
    
  ![alt text](https://github.com/agonzalezramos/Spotify-Recommender/blob/main/img1.png?raw=true)
  ![alt text](https://github.com/agonzalezramos/Spotify-Recommender/blob/main/img2.png?raw=true)
  
 As we can observe, both of the lists have danceability, energy and valence as their main features. However, there are differences related to the intensity of each of them.

  ![alt text](https://github.com/agonzalezramos/Spotify-Recommender/blob/main/img3.png?raw=true)
  
  Another approach that we can do is to compare the mean of each feature between datasets. In this case, danceability and energy are the ones with much more difference on the df_NO, and Acousticness is the main one on the df_SI.

 ## Usage
 
 If you want to use this notebook, simply grab the code from the repo, paste your Spotify Dev Credentials and give it a try. On the other hand, if you want to replicate the model, I have also left the processed final dataframe based on my personal account  (otherwise you wouldn't be able to get my liked songs playlist).


## Useful links

https://developer.spotify.com/documentation/web-api/reference/#/operations/get-audio-features
https://towardsdatascience.com/is-my-spotify-music-boring-an-analysis-involving-music-data-and-machine-learning-47550ae931de Thanks to Juan De Dios Santos
https://towardsdatascience.com/a-music-taste-analysis-using-spotify-api-and-python-e52d186db5fc  Thanks to Jonathan Cabreira
https://www.linkedin.com/pulse/extracting-your-fav-playlist-info-spotifys-api-samantha-jones/ Thanks to Samantha Jones
