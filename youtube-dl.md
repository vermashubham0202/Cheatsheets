# youtube-dl guide (linux tool):
## Display all available format of a video:
```
youtube-dl -F <url>
```
or
```
youtube-dl --list-formats <url>
```
## Download video or playlist:
```
youtube-dl <video_link / playlist_link>
```
## Download multiple videos:
```
youtube-dl <url1> <url2>
```
or put all links in a text file and run below command:
```
youtube-dl -a url.txt
```
## Download youtube playlist with numbering:
```
youtube-dl -o "%(playlist_index)s-%(title)s.%(ext)s" <playlist_link>
```
## Important options:
### --playlist-start
```
youtube-dl <playlist_link> --playlist-start 5
```
<start downloading from video number 5 of playlist>

### --playlist-items
```
youtube-dl <playlist_link> --playlist-items 2, 5-9, 15
```
<download 2nd, from 5th video to 9th video and 15th video>

## Download audio only from a video:
```
youtube-dl -x --audio-format mp3 <url>
```
## Download file at a certain speed (limit download speed) "bytes per second":
```
youtube-dl -r 50K <url>
```
## Download forcefully partially download files (if by-default it is fail to do):
```
youtube-dl -c <url>
```
