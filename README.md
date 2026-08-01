# Video-Archive

This repository contains simple single-file web tools to extract and play media from Archive.org (Internet Archive) and the Wayback Machine (web.archive.org).

Files included:

- wayback-media-extractor.html — Extracts media links from a web.archive.org replay URL and lets you play or open archived media resources.
- archive-archiveorg-player-with-url-extract.html — Search Archive.org, extract an item's identifier from an Archive.org item URL, fetch metadata and list playable files, and play via Archive.org embed or direct file playback.

Usage

1. Clone or download the repo.
2. Open one of the HTML files in a modern browser (Chrome/Firefox). For best results, serve them from a local static server (python -m http.server) to avoid some file:// restrictions.
3. Paste a web.archive.org replay URL into wayback-media-extractor.html and click "Extract media".
4. Paste an archive.org item URL into archive-archiveorg-player-with-url-extract.html and click "Extract from URL".

Notes

- CORS: Some archived pages or resources may block cross-origin requests or embedding (X-Frame-Options). If extraction fails, try opening the replay page in a new tab, or run the included tools from a server or with a simple proxy.
- HLS/DASH: The current tools do not auto-play HLS (.m3u8) or DASH (.mpd) manifests. If you need HLS playback, consider adding hls.js (I can add that on request).

License

MIT
