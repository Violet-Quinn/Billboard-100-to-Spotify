# 🎶 Billboard 100 to Spotify

This Python script scrapes the Billboard Hot 100 for a user-specified date and creates a private Spotify playlist with the top tracks from that day using the Spotify Web API.

---

## Features

- Input a date (YYYY-MM-DD)
- Scrape top 100 songs from Billboard
- Authenticate with Spotify via OAuth
- Create a private Spotify playlist
- Add matching tracks to the playlist

---

## Requirements

- Python 3.7+
- A [Spotify Developer Account](https://developer.spotify.com/dashboard)

---

## Installation

```bash
git clone https://github.com/your-username/billboard-to-spotify.git
cd billboard-to-spotify
pip install -r requirements.txt
```

---

## Setup

  Create a Spotify Developer App:

  - Go to the Spotify Developer Dashboard

  - Create a new app and note down:

      -Client ID

      -Client Secret

      -Redirect URI (e.g., https://example.com)

  - Edit your script:

    Replace the placeholders in your Python code with your credentials:

    YOUR_APP_CLIENT_ID = "your_client_id"
    YOUR_APP_CLIENT_SECRET = "your_client_secret"
    YOUR_APP_REDIRECT_URI = "your_redirect_uri"

---

## Usage

  Run the script:

  ```bash
  python billboard_to_spotify.py
  ```

Enter a date in the format YYYY-MM-DD when prompted.

A Spotify authentication URL will be displayed in the terminal.
Open it in your browser and log in to your Spotify account.

After authentication, Spotify will redirect you to the redirect URI.
Copy the entire URL from the browser and paste it back into the terminal when prompted.

The script will:

  - Scrape Billboard Hot 100 songs from that date

  - Search them on Spotify

  - Create a private playlist

  - Add the matched songs

---


## Notes

  - Not all songs may be found on Spotify, especially older or region-specific ones.

  - The script only adds songs that Spotify returns in search results.

  - If Billboard changes its website structure, the scraper may need to be updated
