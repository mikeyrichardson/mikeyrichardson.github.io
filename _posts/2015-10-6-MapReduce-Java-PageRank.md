---
layout: post
title: Using the Hadoop Java API to Find PageRank
---
One of assignments in the Mining Massive Datasets course is to write a program to compute PageRank given a text file containing a subset of a web graph. ([Here](http://snap.stanford.edu/data/web-Google.txt.gz) is the data.) It didn't take long to write a Python script to efficiently calculate PageRank with Numpy arrays. But I wanted to try writing a program that could scale to graphs that were too big to be contained in the memory of one machine, so I also wrote the program using the Hadoop Java API.

After reading through half of the book *Pro Hadoop*, I decided that I wanted to try writing a Hadoop program using the Java API. I had used Hadoop streaming with Python and wanted to see how much harder it would be to do everything in Java. The PageRank problem seemed like a great opportunity.

It didn't take long to see why using the Java API can be so frustrating. Every change needs to be accounted for in multiple locations of the code and I frequently forgot at least one of them. Progress was much slower than I expected. 

But there were also some benefits to using the Java API. It gave me a lot more appreciation for all of the steps in the Hadoop cycle. I was also learned how to control things like partitioning, grouping, and secondary sorting (even though I eventually realized that I could do everything without such complications).

There are many more optimizations that could be made to the code (such as maintaining copies of the matrix in memory between jobs), but I still haven't figured out how to control things like that.

[View source code](https://github.com/mikeyrichardson/hadoop_page_rank)

 