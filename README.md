# mpd-stickers

This repository is an attempt  to document MPD stickers usage across various MPD client projects. Contributions are very welcome!

The ultimate goal of this project is to create a standard for common sticker names.

## From the MPD documentation

“Stickers” are pieces of information attached to existing MPD objects (e.g. song files, directories, albums; but currently, they are only implemented for song). Clients can create arbitrary name/value pairs. MPD itself does not assume any special meaning in them.

The goal is to allow clients to share additional (possibly dynamic) information about songs, which is neither stored on the client (not available to other clients), nor stored in the song files (MPD has no write access).

Client developers should create a standard for common sticker names, to ensure interoperability.

## Clients with sticker support

- [Cantata](https://github.com/nullobsi/cantata)
- [mpdev](https://github.com/mbhangui/mpdev)
- [myMPD](https://github.com/jcorporation/myMPD)

### Cantata

| Sticker | Format | Description |
| ------- | ------ | ----------- |
| rating | Integer in range 0-10 | 5 Stars rating, with half-stars |

### mpdev

| Sticker | Format | Description |
| ------- | ------ | ----------- |
| rating | Integer in range 0-10 | 5 Stars rating, with half-stars |

### myMPD

| Sticker | Format | Description |
| ------- | ------ | ----------- |
| elapsed | Unix timestamp | Recent song position |
| lastPlayed | Unix timestamp | Last played time of song |
| lastSkipped | Unix timestamp | Last skipped time of songs |
| like | Integer in range 0-2 |0 - dislike, 1 - neutral, 2 - like |
| playCount | Integer | How often the song was played |
| rating | Integer in range 0-10 | 5 Stars rating |
| skipCount | Integer | How often the song was skipped |
