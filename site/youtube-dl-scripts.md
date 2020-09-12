# My `youtube-dl` Scripts


### Youtube Channels - Video

```powershell

youtube-dl --format "(bestvideo[vcodec^=av01][height>=4320][fps>30]/bestvideo[vcodec^=vp9.2][height>=4320][fps>30]/bestvideo[vcodec^=vp9][height>=4320][fps>30]/bestvideo[vcodec^=av01][height>=4320]/bestvideo[vcodec^=vp9.2][height>=4320]/bestvideo[vcodec^=vp9][height>=4320]/bestvideo[height>=4320]/bestvideo[vcodec^=av01][height>=2880][fps>30]/bestvideo[vcodec^=vp9.2][height>=2880][fps>30]/bestvideo[vcodec^=vp9][height>=2880][fps>30]/bestvideo[vcodec^=av01][height>=2880]/bestvideo[vcodec^=vp9.2][height>=2880]/bestvideo[vcodec^=vp9][height>=2880]/bestvideo[height>=2880]/bestvideo[vcodec^=av01][height>=2160][fps>30]/bestvideo[vcodec^=vp9.2][height>=2160][fps>30]/bestvideo[vcodec^=vp9][height>=2160][fps>30]/bestvideo[vcodec^=av01][height>=2160]/bestvideo[vcodec^=vp9.2][height>=2160]/bestvideo[vcodec^=vp9][height>=2160]/bestvideo[height>=2160]/bestvideo[vcodec^=av01][height>=1440][fps>30]/bestvideo[vcodec^=vp9.2][height>=1440][fps>30]/bestvideo[vcodec^=vp9][height>=1440][fps>30]/bestvideo[vcodec^=av01][height>=1440]/bestvideo[vcodec^=vp9.2][height>=1440]/bestvideo[vcodec^=vp9][height>=1440]/bestvideo[height>=1440]/bestvideo[vcodec^=av01][height>=1080][fps>30]/bestvideo[vcodec^=vp9.2][height>=1080][fps>30]/bestvideo[vcodec^=vp9][height>=1080][fps>30]/bestvideo[vcodec^=av01][height>=1080]/bestvideo[vcodec^=vp9.2][height>=1080]/bestvideo[vcodec^=vp9][height>=1080]/bestvideo[height>=1080]/bestvideo[vcodec^=av01][height>=720][fps>30]/bestvideo[vcodec^=vp9.2][height>=720][fps>30]/bestvideo[vcodec^=vp9][height>=720][fps>30]/bestvideo[vcodec^=av01][height>=720]/bestvideo[vcodec^=vp9.2][height>=720]/bestvideo[vcodec^=vp9][height>=720]/bestvideo[height>=720]/bestvideo)+(bestaudio[acodec^=opus]/bestaudio)/best" --sleep-interval 1 --max-sleep-interval 3 --ignore-errors --no-continue --no-overwrites --download-archive archive.log --write-description --all-subs --embed-subs --output "%(uploader)s/%(uploader)s - %(upload_date)s - %(title)s/%(uploader)s - %(upload_date)s - %(title)s [%(id)s].%(ext)s" --merge-output-format mkv --add-metadata --batch-file "Channels.txt"

```

### Youtube Channels - Audio

```powershell

youtube-dl --format "(bestaudio[acodec^=opus]/bestaudio)/best" --verbose --sleep-interval 2 --max-sleep-interval 4 --ignore-errors --no-continue --no-overwrites --download-archive archive.log --add-metadata --write-description --write-info-json --write-annotations --write-thumbnail --extract-audio --output "%(uploader)s/%(uploader)s - %(upload_date)s - %(title)s/%(uploader)s - %(upload_date)s - %(title)s [%(id)s].%(ext)s" --batch-file "Channels.txt"

```

### Youtube Videos - Audio

```powershell

youtube-dl --format "(bestaudio[acodec^=opus]/bestaudio)/best" --verbose --download-archive archive.log --add-metadata --extract-audio -o "%(title)s.%(ext)s" --batch-file "Youtube Videos - Audio.txt"

```

### Crunchyroll Videos

```powershell

youtube-dl --no-check-certificate --add-metadata --all-subs --embed-subs --merge-output "mkv" --batch-file "Crunchyroll - Videos.txt"

```

###  BBC iPlayer Videos

```powershell

youtube-dl -i --all-subs --embed-subs --convert-subs "srt" --merge-output "mkv" --output "%(title)s [%(id)s].%(ext)s" --download-archive archive.log --batch-file "BBC iPlayer Videos.txt"

```

### Soundcloud Music - Tracks



```powershell

youtube-dl --add-metadata --output "%(title)s.%(ext)s" --download-archive archive.log -i --batch-file "Soundcloud - Tracks.txt"

```

### Soundcloud Music - Artists

```powershell

youtube-dl --add-metadata --output "%(uploader)s/%(title)s/%(title)s.%(ext)s" --write-description --write-thumbnail --download-archive archive.log -i --batch-file "Soundcloud - Artists.txt"

```

