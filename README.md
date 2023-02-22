# Spotify-Recommender

  As a musician, I cannot live without my daily dose of a proper Spotify Session. This led me to ask, why not consider using my own data collected along the years, to first make a small exploratory analysis and second, try to develop a classification model that would predict if I liked or not a song.

  In order to achieve my objective, I started to look for previous works already done in the community of Data Scientists (each of them will be quoted at the end), and I discovered that Spotify already has an API that allow us to extract what they call, the “Audio-Features”, which they are certain kind of attributes that belong to each song. For instance, some of them are very subjective fields as, how “danceable” or how much “energy” a song has, and others more objective like Tempo, Key or Mode (minor or major).
  
  Gladly, it exists a Python Library called "Spotipy", that allows us to connect to the API in a easy and quick way. It's worth to mention that it will be require a Spotify "Dev Account", but the process is easy and free of charge.
  
 ## Enviroment
 
 The whole work was done in a Google Colab Jupyter Notebook, with each of the following tools:
 
- A **Dev Account** in Spotify
- **Spotipy** Library for getting our data
-	**Plotly** Library for an interactive data visualization
-	**Pandas** and **Numpy** Library for data analysis
-	**Scikit-Learn** Library for our Machine Learning model

## EDA
  
  We created 2 lists: One based on all the songs that I have liked along the years (df_SI), and other one based in all genres that I really do not like as “Reggaeton” and “Cumbia 420” (df_NO).  Each of them has 400 songs, and here there are some facts about ther features.
    
  ![alt text](https://github.com/agonzalezramos/Spotify-Recommender/blob/main/img1.png?raw=true)
  ![alt text](https://github.com/agonzalezramos/Spotify-Recommender/blob/main/img2.png?raw=true)
  
  As we can observe, both of the lists have “danceability”, “energy” and “valence” as the main features, however there are differences related of the intensity of each of them.

  ![alt text](https://github.com/agonzalezramos/Spotify-Recommender/blob/main/img3.png?raw=true)
  
  Another approach that we can do is to compare the mean of each feature between datasets. In this case, “danceabilty” and “energy”  are the ones with much more difference on the df_NO, and “Acousticness” is the main one on the df_SI. 

 ## Usage
 
If you want to use this notebook, simply paste your Spotify Dev Credentials and give it a try.
On the other hand, if you want to replicate the model, I have left the procesed final dataframe based on my personal account (otherwise you wouldn't be able to get my liked songs playlist).

## Useful links

https://developer.spotify.com/documentation/web-api/reference/#/operations/get-audio-features
https://towardsdatascience.com/is-my-spotify-music-boring-an-analysis-involving-music-data-and-machine-learning-47550ae931de Thanks to Juan De Dios Santos
https://towardsdatascience.com/a-music-taste-analysis-using-spotify-api-and-python-e52d186db5fc  Thanks to Jonathan Cabreira
https://www.linkedin.com/pulse/extracting-your-fav-playlist-info-spotifys-api-samantha-jones/ Thanks to Samantha Jones
