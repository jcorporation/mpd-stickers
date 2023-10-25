# mpd-stickers

This repository is an attempt  to document MPD stickers usage across various MPD client projects. Contributions are very welcome!

The ultimate goal of this project is to create a standard for common sticker names.

## From the MPD documentation

“Stickers” 2 are pieces of information attached to existing MPD objects (e.g. song files, directories, albums; but currently, they are only implemented for song). Clients can create arbitrary name/value pairs. MPD itself does not assume any special meaning in them.

The goal is to allow clients to share additional (possibly dynamic) information about songs, which is neither stored on the client (not available to other clients), nor stored in the song files (MPD has no write access).

Client developers should create a standard for common sticker names, to ensure interoperability.

## Clients with sticker support

- [Cantata](https://github.com/CDrummond/cantata)
- [mpdev](https://github.com/mbhangui/mpdev)
- [myMPD](https://github.com/jcorporation/myMPD)

### Cantata

Archived, is there any maintained fork?

| Sticker | Format | Description |
| ------- | ------ | ----------- |
| rating | integer in range 0-10 | 5 Stars rating, with half-stars |

### mpdev

| Sticker | Format | Description |
| ------- | ------ | ----------- |
| rating | integer in range 0-10 | 5 Stars rating, with half-stars |

### myMPD

| Sticker | Format | Description |
| ------- | ------ | ----------- |
| elapsed | unix timestamp | recent song position |
| lastPlayed | unix timestamp | last played time of song (unix timestamp) |
| lastSkipped | unix timestamp | last skipped time of songs (unix timestamp) |
| like | integer in range 0-2 |0 - dislike, 1 - neutral, 2 - like |
| playCount | integer | How often the song was played |
| skipCount | integer | How often the song was skipped |
