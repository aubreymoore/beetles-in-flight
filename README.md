## Technical notes

### UV project initiation
```
uv init --python 3.10 beetles-in-flight
cd beetles-in-flight
uv venv .venv
source .venv/bin/activate
uv add --dev ipykernel
uv add yt-dlp
```

### yt-dlp
The YouTube download program, ```yt-dlp```, is used to download the best quality video-only version of the online video ([reference](https://ostechnix.com/yt-dlp-tutorial/)). 
```
yt-dlp -f bestvideo https://www.youtube.com/watch?v=IUQSZHr9h9Q 
```