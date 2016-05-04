---
layout: post
title:  "Timed Programming and Side Projects"
date:   2016-05-02 08:46:47 -0700
categories: general
---

A general update for this week.

#### Programming Challenge
My attention was recently brought to web services like HackerRank, which provide
time-based programming challenges. The challenges are interesting and fun to 
approach, but I have minimal experience "programming for time." I am excited to
see how that will change in the coming weeks. I may post solution snippets in
the blog if appropriate. 


#### Audiobook Project
The audioreader prototype was completed about a week ago and has been in use
since. Unfortunately, I have not had time to exhaustively test the prototype.
Before I get back to testing, I will clean up the implementation slightly. 
For now, the calculation is off by ~5 pages on average. This is due to 
underlying issues in comparing audiobooks to actual prints. To name a few:

+ Books have pages dedicated to maps, images, table of contents, etc. and 
narrators seldom verbalize this information (intro/outro biases)

+ There are page gaps at the end of chapters that narrators can ignore

+ Assume narrators read at different paces and audiobook files are 
organized differently for every series

It is also worth noting I have issues with the fact that I am testing this 
prototype on a single series. I would like to use this in the long run, and
it wont do if I have to modify source for each series. I need to find a 
solution for automating this process with audibooks and eBooks, so I can 
quickly gather average values for the offsets and biases. At later point,
I can use the averages to (hopefully) get closer to the actual page. I will
also be adding a manual tuning feature for special situations. 






