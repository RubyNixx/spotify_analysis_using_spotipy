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
cd spotify-listening-stats

  2. Set up your Spotify Developer account:

*    Go to the Spotify Developer Dashboard
*   Create a new app
*   Note your Client ID and Client Secret
*   Add http://localhost:8888/callback as a Redirect URI in your app settings

  3. Set environment variables with your Spotify credentials:
<b>Do not share your API client ID or client secret on Github</b>
export SPOTIPY_CLIENT_ID='your-client-id'
export SPOTIPY_CLIENT_SECRET='your-client-secret'
export SPOTIPY_REDIRECT_URI='http://localhost:8888/callback'

4. Run the main script in google colab
