---
title: Playlist Maker
author: Ryan Anderson
created: 2021-09-19
updated: 2021-09-19
version: 0.1.0
---

# Playlist Maker (name TBD)

This is a project to create random music playlists based on artists performing at venues in a certain area and a certain time period. It does this by scraping sites with concert information (either aggregated or directly from venues) and create Spotify playlists based on the artists playing. This is done to help music fans (like myself) explore new artists and new venues in their area or city with a sampling of songs from all artists instead of looking for specific acts they want to see.

## Current method

- Scrape an aggregated site (like [Early Warnings](https://chicagoreader.com/earlywarnings/previously-listed/))
- Update a database with artists, venues, and dates
- Create CLI to accept area and location
- Connect to Spotify API
- Create empty playlist based on user (or just use my own as default)
- Hit API with artists and get sample of 4-5 songs
- Update playlist with songs
- Create separate file (maybe in playlist description) to summarize artists, venues, genres, and dates

## TODO

### Overhead

- Create Dockerfile
- Create Poetry project
- Update requirements in README
- Create *How to run* in README
- Get Spotify API key

### Code stuff

- Create database and migrations
- Scrape aggregated site for data
- Write data to database
- Pass Spotify API key in environment
- Create playlist using API key
- Create CLI to accept location and time period parameters
- Hit API using parameters
- Get 4-5 songs (most popular and some rando too?)
- Add songs to playlist
- Add extra info to description and output in text or stdout
