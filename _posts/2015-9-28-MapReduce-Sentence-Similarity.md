---
layout: post
title: MapReduce to Find Similar Sentences
---

This project aims to find similar pairs of sentences using MapReduce. Both of the scripts use mrjob to create MapReduce chains.

  * The script `find_jaccard_similar_sentences.py` finds sentences which are deemed similar based on minhash estimates of jaccard similarity.
  * The script `find_edit_distance_at_most_one.py` finds sentences that have edit distance at most one by creating hashes of sentence halves to group similar sentences.

[View source code](https://github.com/mikeyrichardson/mapreduce_jaccard_similarity/)  
