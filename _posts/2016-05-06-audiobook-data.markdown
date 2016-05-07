---
layout: post
title:  "Epub Scanning & Speech-To-Text"
date:   2016-05-06 07:01:11 -0700
categories: audiobook

---

I will be exploring epub and speech-to-text modules to help automate tests
of correctness for the audioreader prototype. 

#### Project Update: Comparing Epubs and MP3s

The audioreader prototype has not changed greatly since the last post. The 
current issue is dealing with program correctness. The only way I can
validate program output is by flipping through a copy of the book I am 
interested in, but this can be automated somehow. 

I am thinking of exploring speech-to-text conversion in Python, though
I currently know nothing about it. If it goes as planned, I will
have several ideas for improving the audioreader in the near future. 
Of course, for any of this to be automated, I also need a means to read
text from .epub files.. 

+ Find means to scan and parse .epub data
+ Transcribe current audio file or listen to narrator's playback (former
more portable) using Sphinx or Google Speech
+ Treat epub data as contiguous blocks to minimize time searching for a 
match on the text (also lowers risk of false positives)





