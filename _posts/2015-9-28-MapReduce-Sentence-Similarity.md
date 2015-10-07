---
layout: post
title: MapReduce to Find Similar Sentences
---

I'm currently working through the course material from Coursera's Mining Massive Datasets and I wanted to explore using MapReduce to determine Jaccard similarity. Recently, I  downloaded a Yelp dataset from [here](http://www.yelp.com/dataset_challenge) to start practicing some NLP. While on Yelp's website, I stumbled across a page mentioning mrjob which is an open source tool created by Yelp as "the easiest route to writing Python programs that run on Hadoop." 

I was intrigued and decided to use mrjob to create a script that can pair sentences based on Jaccard similarity. I also used it to complete an optional assignment from the Mining Massive Datasets course (an assignment to find sentences that differ at most by a word edit distance of one).

I enjoyed using mrjob and am planning to try my next project using Hadoop and Java. I want to truly appreciate the ease of Hadoop streaming and Python.

[View source code](https://github.com/mikeyrichardson/mapreduce_jaccard_similarity/)  
