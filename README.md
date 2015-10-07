A Spotify Playlist Duplicator
=============================

Have you ever wanted to remove duplicated tracks from your Spotify Playlists?
Now you can detect and remove them using Spotify dedup.

This project uses the [Spotify Web API](https://developer.spotify.com/web-api/) for managing playlists. Just log in and it will traverse your playlists, finding tracks that appear multiple times with the same identifier (Spotify URI) in a given playlist.

If it finds duplicates, they can be removed just pushing a button. And since it doesn't create a whole new playlist, it keeps its followers.

## Try it
You can check it out on [http://jmperezperez.com/spotify-dedup/](http://jmperezperez.com/spotify-dedup/) or run it locally.

## Install and run
Install the dependencies:

    npm install

Run it:

    grunt serve

## About the Spotify Web API

This app is a good example of how to traverse a user's library without incurring in rate limit. Have a look at the code and see how Promises and a Promise Queue are used to control the amount of requests sent to the Spotify Web API.
