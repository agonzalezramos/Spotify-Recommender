# Spotify-Recommender

  As a musician, I cannot live without my daily dose of a proper Spotify Session. This led me to ask, why not consider using my own data collected along the years, to first make a small exploratory analysis and second, try to develop a classification model that would predict if I liked or not a song.

  In order to achieve my objective, I started to look for previous works already done in the community of Data Scientists (each of them will be quoted at the end), and I discovered that Spotify already has an API that allow us to extract what they call, the “Audio-Features”, which they are certain kind of attributes that belong to each song. For instance, some of them are very subjective fields as, how “danceable” or how much “energy” a song has, and others more objective like Tempo, Key or Mode (minor or major).
  
  Gladly, it exist a Python Library called "Spotipy", that allow us to connect to the API in a easy and quick way. It's worth to mention that it will be require a Spotify "Dev Account", but the process is easy and free of charge.
  
 ## Enviroment
 
 The whole work was done in a Google Colab Jupyter Notebook, with each of the following tools:
 
- A **Dev Account** in Spotify
- **Spotipy** Library for getting our data
-	**Plotly** Library for an interactive data visualization
-	**Pandas** and **Numpy** Library for data analysis
-	**Scikit-Learn** Library for our Machine Learning model

 ## Usage
 
If you want to use this notebook, simply paste your Spotify Dev Credentials and give it a try.
On the other hand, if you want to replicate the model, I have left the procesed final dataframe based on my personal account (otherwise you wouldn't be able to get my liked songs playlist).

## Useful links

https://developer.spotify.com/documentation/web-api/reference/#/operations/get-audio-features
https://towardsdatascience.com/is-my-spotify-music-boring-an-analysis-involving-music-data-and-machine-learning-47550ae931de Thanks to Juan De Dios Santos
https://towardsdatascience.com/a-music-taste-analysis-using-spotify-api-and-python-e52d186db5fc  Thanks to Jonathan Cabreira
