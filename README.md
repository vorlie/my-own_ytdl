# IMPORTANT!!
If your antivirus is gonna complain about the .exe, you can ignore it! It's false positive I tried everything I could to make it not complain! [VirusTotal result](https://www.virustotal.com/gui/file/33c355e4989ab3164d1bfca6c576fa95e9f8f6c0e80d5e7a606138df9c49f20e/detection)

# Requirements
- Windows 10+
- Python 3.12 (Optional)
 - scdl `pip install scdl` (Optional)

> scdl is required only when you want to download songs from soundcloud, if you don't want then you don't need to install it!

# Dependencies
- yt-dlp
- ffmpeg/ffprobe
- scdl (optional)

## Build it yourself
Use [Pyinstaller](https://pypi.org/project/pyinstaller/)
Check the [.spec file](https://github.com/vorlie/YoutubeDL/blob/main/spec-file-example-for-windows.spec) and specify the paths for the required datas. 
Once you do, run `pyinstaller name-of-the-spec-file.spec`

These will append the required files to the .exe
```
datas=[
    ('PATH-TO-THIS-FOLDER\\assets', 'assets'),
    ('PATH-TO-THIS-ICON\\icon.ico', '.'),
    ('PATH-TO-THIS-FOLDER\\dependencies', '.')
]
```

## Gallery
![https://cx.tixte.co/r/preview-ytdl.png](https://cx.tixte.co/r/preview-ytdl.png)
