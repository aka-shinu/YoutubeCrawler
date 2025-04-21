# 🎥 YouTubeCrawler: Python Wrapper for YouTube Scraping

A user-friendly and feature-rich Python wrapper to extract detailed information about **YouTube videos and channels**.

📚 **Readable and well-documented:**  
👉 [GitHub Repository](https://github.com/KeinShin/youtubecrawler)

---

## 🚀 Installation

```bash
pip3 install youtubecrawler
```

---

## 📦 Initialization

```python
from youtubecrawler import crawl

# Using video name
yt = crawl(video_name="xyz")

# Or using video link
yt = crawl(video_link="https://youtube.com/xyz")

# Or using video ID
yt = crawl(video_id="abc123")
```

---

## 🎬 Video Features

You can extract all details in one go or call them individually.

### ✅ Get All Video Details

```python
video = yt.VideoDetails()
```

### ✅ Individual Info

```python
views = yt.views()
tags = yt.keyword()
link = yt.videolink()
likes = yt.likes_dislikes()[1]
dislikes = yt.likes_dislikes()[2]
upload_time = yt.videoUploadTime()
title = yt.VidTitle()
description = yt.description()
uploader = yt.channel()
```

---

## 📺 Channel Features

### ✅ Initialization

```python
from youtubecrawler.channel import channel

# Using channel name
ch = channel(channelname="CarryMinati")

# Using channel link
ch = channel(channellink="https://youtube.com/@carryminati")

# Using channel ID
ch = channel(channelid="/channel/UC0IWRLai-BAwci_e9MylNGw")
```

### ✅ Channel Info

```python
subs = ch.subs()                      # Get subscriber info
latest_video = ch.latest_video()     # Latest video details
post = ch.latest_community()         # Latest community post
other_channels = ch.spareChannels()  # Linked channels
about_links = ch.links()             # Links in About section
```

---

## ✅ Summary

- 📹 Get video stats, uploader info, and content details
- 📡 Scrape channel metadata, community posts, linked channels, etc.
- 🛠 Built for flexibility: Use name, link, or ID as input
- 🔥 Ideal for YouTube data scraping, automation, and analytics

---

## 🧑‍💻 Author

Made with ❤️ by KeinShin  
📌 [GitHub: KeinShin](https://github.com/KeinShin)
