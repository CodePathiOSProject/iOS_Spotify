Original App Design Project - README Template
===

# Spotify

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
1. [Schema](#Schema)

## Overview
### Description
App will essentially be a clone of Spotify. Users will be able to log in and see their "Favorite" songs and playlists, and users will be able to add songs to both lists. Users should also be able to search for artists. Song-playing functionality may be included.

### App Evaluation

- **Category:** Music
- **Mobile:** App will involve audio, push mechanisms, and real-time features. 
- **Story:** Allows users to listen to music and organize music according to preference
- **Market:** Anybody who enjoys listening to music will enjoy this app.
- **Habit:** An average user likely use this app often but along with something else, as it is mostly for music. The average user would also only consume content.
- **Scope:** Spotify only features music-related content; this app will form a basic version of that with no extra features.

## Product Spec

### 1. User Stories (Required and Optional)

**Required Must-have Stories**

* Sign-In/Sign-Out with Spotify
* Search the music
* Add or remove music to the list
* Search for artists

**Optional Nice-to-have Stories**

* Song-playing 
* ...

### 2. Screen Archetypes

* Login Screen
   * User enters username/email and password
* Home Screen
   * User can view recently played, new releases, etc.
* Search Screen
   * User can search for songs, artists, playlosts, etc.
* Library
   * User can view playlists
* Song screen
    * User views details about the song and can choose to play
* Song Playing Screen (maybe)
    * User can see album cover and song runtime

### 3. Navigation

**Tab Navigation** (Tab to Screen)

* Home Screen
* Search Screen
* Library

**Flow Navigation** (Screen to Screen)

* Login Screen
   * Home Screen
* Home Screen/Library
   * Song Screen (when song or playlist is clicked)
* Home, Search, Library
    * Song Playing Screen
        * When bottom bar showing song is clicked

## Wireframes
[Add picture of your hand sketched wireframes in this section]
<img src="img1.png" width=600>
<img src="img2.jpg" width=600>

### [BONUS] Digital Wireframes & Mockups

### [BONUS] Interactive Prototype

## Schema 
### Models
[Add table of models]
#### Post

   | Property      | Type     | Description |
   | ------------- | -------- | ------------|
   | song     | String   | song name |
   | artist        | String| song artist |
   | image         | File     | song image (album cover or NA if none) |
   | releaseDate       | DateTime   | song release date |
   | likesCount    | Number   | number of likes for the song |
### Networking
- [Add list of network requests by screen ]
- [Create basic snippets for each Parse network request]
- [OPTIONAL: List endpoints if using existing API such as Yelp]
#### List of network requests by screen
   - Home Feed Screen
      - (Read/GET) Query all songs where user is artist
      - (Create/POST) Create a new like on a song
      - (Delete) Delete existing like on song
   - Create Post Screen
      - (Create/POST) Create a new song object
   - Profile Screen
      - (Read/GET) Query logged in user object
#### [OPTIONAL:] Existing API Endpoints
##### Spotify Web API
- Base URL - [https://developer.spotify.com/documentation/web-api/](https://developer.spotify.com/documentation/web-api/)

   HTTP Verb | Endpoint | Description
   ----------|----------|------------
    `GET`    | /song/url | gets song url
    `GET`    | /song | gets song name

![](https://github.com/CodePathiOSProject/iOS_Spotify/blob/main/ezgif.com-gif-maker%20(7).gif)

**Sprint 1 User Stories**

Time spent: **x** hours spent in total

- [ ] User sees app icon in the home screen
- [x] User sees load screen with logo
- [x] User is directed to login screen on launch
- [ ] User can create an account
- [ ] User can log in
