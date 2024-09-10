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

git clone https://github.com/RubyNixx/spotipy_user_analysis.git

2. Set up your Spotify Developer account:

*    Go to the Spotify Developer Dashboard
*   Create a new app
*   Note your Client ID and Client Secret
*   Add http://localhost:8888/callback as a Redirect URI in your app settings

3. Set environment variables with your Spotify credentials:
<b>Do not share your API client ID or client secret on Github</b>

To handle this, i've used files with enviroment variables (.env) and utilised a .gitignore file to ensure sensitive information isnt included. I've then set and called them as variables within the python code.

export SPOTIPY_CLIENT_ID='your-client-id'
export SPOTIPY_CLIENT_SECRET='your-client-secret'
export SPOTIPY_REDIRECT_URI='http://localhost:8888/callback'

4. Run the main script in google colab

5. On first run, you'll be prompted to authorise the app to access your Spotify data. Follow the link provided to complete the authorisation process.

6. Sample Outputs:

![spotipy1](https://github.com/user-attachments/assets/6d96f552-314f-4039-a236-cf2182cb2ee0)

![spotipy2](https://github.com/user-attachments/assets/8346eab9-e412-4d0e-b6ce-4965b254605a)

![spotipy3](https://github.com/user-attachments/assets/6700eb9d-ca7d-495e-9532-7a300557b0e1)

![ShortTermVsLongTerm](https://github.com/user-attachments/assets/d62abd60-93f1-4aea-b6cf-7176c194130e)

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
https://stmorse.github.io/journal/spotify-api.html

https://github.com/spotipy-dev/spotipy-examples/blob/main/showcases.ipynb
