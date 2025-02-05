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

### git
```uv``` set up a local repository, ```.git```, when the project is initiated.
The local repo was initiated using:
```
git add .
git commit -m 'initial'
```

I then crated a new GitHub repo connected it to my local repo using:
```
git remote add origin https://github.com/aubreymoore/beetles-in-flight.git
git branch -M main
git push -u origin main
```

### yt-dlp
The YouTube download program, ```yt-dlp```, is used to download the best quality video-only version of the online video ([reference](https://ostechnix.com/yt-dlp-tutorial/)). 
```
yt-dlp -f bestvideo https://www.youtube.com/watch?v=IUQSZHr9h9Q 
```

### opencv (cv2)
```
uv add opencv-python
```