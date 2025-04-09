# Time Machine Project

This project allows you to create a playlist on Spotify based on the Billboard Hot 100 chart from a specific date in the past. You can input any date in the `YYYY-MM-DD` format, and the script will scrape the Billboard website for that day's Hot 100 song list, search for each song on Spotify, and create a private playlist with those tracks.

## Features

- **Billboard Chart Scraping**: Scrapes the Billboard Hot 100 chart for a specific date.
- **Spotify Integration**: Authenticates with Spotify API to search for songs and create a playlist.
- **Private Playlist Creation**: Automatically creates a private Spotify playlist with songs from the specified Billboard chart.

## Requirements

- Python 3.6 or higher
- Spotify Developer account and credentials (Client ID and Secret)
- The following Python libraries:
  - `requests`
  - `beautifulsoup4`
  - `spotipy`

You can install these dependencies using `pip`:

```bash
pip install requests beautifulsoup4 spotipy
```

## Setup

1. **Spotify Developer Account**: 
   - Go to [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/applications) and log in with your Spotify account.
   - Create a new application to get the `Client ID` and `Client Secret` required for authentication.
   
2. **Get the Credentials**:
   - Replace the `ID` and `SECRET` variables in the script with your own `Client ID` and `Client Secret` from the Spotify Developer Dashboard.

3. **Run the Script**:
   - Simply run the script in your Python environment:
   ```bash
   python main.py
   ```
   - It will ask you to input a date in the format `YYYY-MM-DD`.
   - The script will scrape the Billboard Hot 100 chart for that date, search for the songs on Spotify, and create a new private playlist with those tracks.

4. **Spotify Authentication**:
   - The script will open a Spotify login page in your browser for authentication.
   - After successfully logging in, the script will proceed to create the playlist.

## Example

1. Run the script:
   ```bash
   python main.py
   ```

2. Input a date when prompted:
   ```text
   Which year do you want to travel to? Type the date in this format YYYY-MM-DD: 2000-12-25
   ```

3. After the script completes, a new private Spotify playlist with the top 100 songs from that date will be created in your account.

## License

This project does not have a license.

## Contributing

Feel free to submit issues or pull requests for any improvements or fixes.
