# MACFlix

## About

This app is a clone of the Netflix frontend (Javascript and React), but consumes the Youtube API and exclusively displays the contents of the CMAC Youtube channel (CmacTv).

The Community Media Access Collaborative (CMAC) is a membership-based, 501(c)(3) non-profit organization created to help citizens, schools, non-profits, public agencies and others better connect with our Fresno/Clovis (California) community through the use of media. 

https://cmac.tv/

## Usage

1. Clone the repo
2. Create a .env file in the project root and add your Youtube API key
	- REACT_APP_YOUTUBE_API_KEY=[your API key]
3. Access index.html in a browser or deploy to your website.

## Documentation

_Features_

- All features are limited to the CmacTV YouTube channel
- Suggest Youtube playlists in the same way netflix suggests genres
- Search bar that searches the channel
- The red tones in the Netflix design are replaced with blue to match CMAC's color scheme
- Clicking on a thumbnail will bring up a hero banner of the video that loops the first 10 seconds, overlaid with:
	- the description and likes
	- play button
	- close button
	- mute toggle button
- start the video from the beginning if the play button or large thumbnail is clicked
- auto-queue the next video if the video was part of a playlist or...
	- play the next suggested video (is this in the api?)
- "Still watching?" prompt after 3 auto-play videos

## Notes

- From stackoverflow: YouTube doesn't expose fullscreen in their API, but you can call the native browser requestFullScreen() function from the playerStateChange() event from the YouTube API or make your own custom play button
