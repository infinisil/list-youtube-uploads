# list-youtube-uploads

A very simple bash script for listing all uploads of a youtube channel.

Has to use web scraping to get the channel id from a channel url. But uses the
YouTube API for actually listing the videos.

## Usage

- Go to the channel url you want to get a list of videos from
- Copy the url
- Call `./list-youtube-uploads` with the url as an argument

The script returns only urls on stdout, but progress information on stderr

Example:
```
$ ./list-youtube-uploads https://www.youtube.com/c/KRAZAM
Channel ID for Channel url https://www.youtube.com/c/KRAZAM is.. UCgBVkKoOAr3ajSdFFLp13_A
Upload playlist ID for channel ID UCgBVkKoOAr3ajSdFFLp13_A is.. UUgBVkKoOAr3ajSdFFLp13_A
Listing all videos..
https://youtube.com/watch?v=67sfZfreOrU
https://youtube.com/watch?v=IZN7Qo6mtSc
https://youtube.com/watch?v=QG_-1RaX8Oo
https://youtube.com/watch?v=WqjUlmkYr2g
https://youtube.com/watch?v=y8OnoxKotPQ
https://youtube.com/watch?v=ICp2-EUKQAI
https://youtube.com/watch?v=xubbVvKbUfY
https://youtube.com/watch?v=P8KaTrGpGg0
https://youtube.com/watch?v=FDoH15ylAeo
https://youtube.com/watch?v=_o7qjN3KF8U
https://youtube.com/watch?v=duJwGSUhRQA
https://youtube.com/watch?v=tndAVl6iGnk
https://youtube.com/watch?v=CJwPb_76jqU
https://youtube.com/watch?v=eSqexFg74F8
https://youtube.com/watch?v=puDMBSieTe0
Listed 15 / 15
All videos listed
```
