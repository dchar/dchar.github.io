---
layout: post
title:  "Side Project"
date:   2016-04-28 08:46:47 -0700
categories: audiobook
---

Reading is one of my favorite hobbies, but I still listen to audiobooks 
because time is a limiting factor during University studies. I see an 
issue with switching between books and audiobooks that can be solved in a few
ways. 

Oftentiems, I listen to audiobooks in place of music when I can. This way,
I do not have an excuse to abandon my book on days I have determined too
busy for reading. Unfortunately, when I want to read, I have difficulty 
finding my location in the physical copy. This issue could be easily 
prevented, say, if there were as many chapters as there were files, but that
is seldom the case. In response, I started working on a Python prototype for
using the reader's audiobook progress to infer an approximate page number
within a physical copy. 

This prototype has two main components: one meant for scanning all .mp3 files
within a directory, and another meant for pulling XML information from a 
locally hosted VLC Media Player session. For reasons currently unknown, all 
.mp3 files were observed to have durations that were 13 seconds longer than
they should have been based on calculations by hand. This is currently being
reflected as an .mp3 bias. The request_position() method goes on to parse the
XML string, storing the track position and track number for later use in 
approximating page number




