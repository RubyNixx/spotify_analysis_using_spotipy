<b>Spotify Listening Stats</b>

This project uses the Spotipy library in Google Colab to analyse personal Spotify listening data and provide headline statistics on listening activity.

<b><i>Features</i></b>

*   Retrieves your top tracks and artists over different time ranges
*   Calculates average audio features (danceability, energy, etc.) of your most-played tracks
*   Generates a breakdown of your listening habits by genre
*   Visualizes listening trends over time

<b><i>Prerequisites</i></b>

*   Python 3.7+ (I used Google Colab)
*   A Spotify account
*   Spotify Developer credentials (Client ID and Client Secret)

<b><i>Setup</i></b>

1. Clone this repository:

[![Clone](https://img.shields.io/badge/Clone-Repository-blue?style=for-the-badge&logo=github)](https://github.com/RubyNixx/spotify_analysis_using_spotipy.git)

2. Set up your Spotify Developer account:

*    Go to the Spotify Developer Dashboard
*   Create a new app
*   Note your Client ID and Client Secret
*   Add http://localhost:8888/callback as a Redirect URI in your app settings

3. Set environment variables with your Spotify credentials:
<b>Do not share your API client ID or client secret on Github</b>

To handle this, i've used files with enviroment variables (.env) and utilised a .gitignore file to ensure sensitive information isnt included. I've then set and called them as variables within the python code.

Create a .env file and store in a secure place. See these instructions how to create a .env file:
https://github.com/RubyNixx/spotify_analysis_using_spotipy/blob/main/Steps_to_create_env_file.md

4. Run the main python script in google colab

   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RubyNixx/spotify_analysis_using_spotipy/blob/main/spotipy.ipynb)


6. On first run, you'll be prompted to authorise the app to access your Spotify data. Follow the link provided to complete the authorisation process.

7. Sample Outputs:

![spotipy2](https://github.com/user-attachments/assets/8346eab9-e412-4d0e-b6ce-4965b254605a)

![spotipy_energy_dist](https://github.com/user-attachments/assets/33499f9f-a689-46ee-bd57-16c4ecf3b629)

![spotipy_top_tracks](https://github.com/user-attachments/assets/a9640325-4d20-43e8-88c3-2862055d246c)

![spotipy_top_50](https://github.com/user-attachments/assets/858d3781-8bef-4655-b4a3-71cf51450308)

![spotipy5](https://github.com/user-attachments/assets/504ff13e-4b02-4827-9078-faa1331af390)

![ShortTermVsLongTerm](https://github.com/user-attachments/assets/d62abd60-93f1-4aea-b6cf-7176c194130e)

![spotipy6](https://github.com/user-attachments/assets/9513dd0c-a987-4cfa-a9e2-747ab8d021db)

![spotipy7](https://github.com/user-attachments/assets/6c5ee392-a052-4cf9-8a52-970098058696)

![spotipy8](https://github.com/user-attachments/assets/623cd09a-9315-47f1-953a-e3d56d06ac32)

The Spotipy library offers several key features for interacting with the Spotify Web API:

*    Full API access: Spotipy provides access to all endpoints of the Spotify Web API, allowing you to retrieve a wide range of music data

*    User authorisation support: The library supports both the Authorization Code flow and the Client Credentials flow for user authentication

*    Lightweight and easy to use: Spotipy is designed to be a lightweight Python wrapper for the Spotify Web API, making it simple to integrate into your projects

*    Comprehensive data retrieval: You can fetch information about artists, albums, tracks, playlists, user profiles, and more

*    Search functionality: Spotipy allows you to search for items in the Spotify catalog

*    Playlist management: You can create, modify, and delete playlists, as well as add or remove tracks

*    User library interactions: The library enables you to access and modify a user's saved tracks and albums

*    Audio features and analysis: You can retrieve audio features and detailed audio analysis for tracks

*    Personalisation: Spotipy provides access to personalized data such as a user's top artists and tracks

*    Follow/unfollow functionality: You can manage following/unfollowing artists, users, and playlists

*    Browse and recommendations: The library allows you to access Spotify's browse and recommendation features

*    Error handling: Spotipy includes built-in error handling for API requests

More information can be found here: 
<b>Spotipy API documentation:</b>
https://spotipy.readthedocs.io/en/2.24.0/
  Note: This will help with understanding the API & how to connect to it. I've included a clause in the python code to help work with the API in a google colab notebook.

<b>Spotipy githib repo:</b>
https://github.com/spotipy-dev/spotipy

<b>Spotipy scopes:</b>
https://developer.spotify.com/documentation/web-api/concepts/scopes#user-top-read

<b>Stack overflow thread that helped with audio features:</b>
https://stackoverflow.com/questions/38823403/scrape-deep-audio-features-using-spotipy-python-library

<b>Exploring features of Spotify playlists - data collection code:</b>
https://orda.shef.ac.uk/articles/code/Exploring_features_of_Spotify_playlists_data_collection_code/19107998

<b>Other github repo inspiration utilising the API:</b>
Using approaches likes PCA to reduce dimensions of data:
https://stmorse.github.io/journal/spotify-api.html

Some examples of how others have used it:
https://github.com/spotipy-dev/spotipy-examples/blob/main/showcases.ipynb
