# YouTube Clip Recorder V2

This Chrome-based local app records a selected section of a YouTube video.

## Start it on macOS

1. Double-click `start.command`.
2. If macOS blocks it, right-click it, choose **Open**, then confirm **Open**.
3. Chrome should open `http://localhost:8080` automatically.

You can also start it manually from this folder:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080` in Chrome.

## Recording

1. Paste a YouTube URL.
2. Enter the start and end times.
3. Click **Load Video**, then **Record Clip**.
4. In Chrome, choose **This Tab** and enable **Share tab audio**.
5. Do not move the mouse during the short preparation period.

V2 starts playback 2 seconds before the requested timestamp. Those preparation seconds are not recorded. The recording begins at the requested start time and stops automatically at the end time.

## Notes

- The cursor is hidden with both a capture preference and a page-level fallback.
- YouTube controls and the app interface are hidden during recording.
- Chrome may save as MP4 or WebM depending on the codecs supported by your version.
- Use only videos you own or have permission to record.
