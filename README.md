# Project Name: spotifyPlaylistScrape

## Overview
The spotifyPlaylistScrape project is developed for CS 105 and is designed to scrape people's Spotify playlists.

## Dependencies
This project heavily depends on Spotipy, which can be found at https://github.com/plamere/spotipy. Additionally, the project requires a client ID and secret from a developer account on Spotify. These can be set in the code or via environmental variables.

## Development Procedure
The development procedure for the project involved implementing the following steps:

1. Created a scraping utility module `scrapeUtil.py` to handle Spotify authentication and token retrieval.
2. Developed a script `harvest.py` to scrape and analyze people's Spotify playlists using the Spotipy library and the authentication utility from `scrapeUtil.py`.
3. Utilized a while loop to iterate through different user IDs and retrieve their playlist information.
4. Handled exceptions for cases where a user ID does not exist or has private playlists.
5. Wrote the retrieved information into a CSV file `results.csv`.
6. Tested and iteratively debugged the script to ensure proper scraping functionality.

## Encountered Errors
During the development process, the following errors were encountered:

1. **Authorization Error**: At the initial stage of development, errors related to unauthorized access to the Spotify API were encountered. This was resolved by implementing the authentication function in `scrapeUtil.py` and ensuring proper handling of the access token.

2. **User Not Found**: While iterating through different user IDs, errors related to users not being found or having private playlists were encountered. This was addressed by implementing exception handling and error-based iteration to continue the scraping process.

## Conclusion
The project successfully implements a scraping mechanism to retrieve information from Spotify playlists. Future development plans may involve further data analysis and visualization of the retrieved playlist data.

