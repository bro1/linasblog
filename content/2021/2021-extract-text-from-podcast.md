---
title: Extract text from podcast
summary: Extract text
author: Linas
date: 2021-06-20T15:00:35.745+13:00
categories:
  - posts
tags:
  - geek

---

Process outline:
1. Download podcast episode in mp3 format
2. Use ffmpeg to convert podcast to a video
3. Upload to youtube
4. Wait - let youtube autogenerate the subtitles
5. Download the subtitles using youtube-dl
6. youtube-dl --write-auto-sub https://www.youtube.com/watch?v=dJtZ8YGyxt
7. Convert the resulting vtt file to text using vtt3text.py


If you are a fan of podcast and want to have a way to search for an episode - post it online (on a blog or a wiki).
