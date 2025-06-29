---
title: "Improving Embedding-Based Retrieval in Friend Recommendation with ANN Query Expansion."
collection: publications
permalink: /publication/sigir_2024
excerpt: "Pau Kung, Zihao Fan, Tong Zhao, Yozen Liu, Zhixin Lai, Jiahui Shi, Yan Wu, Jun Yu, Neil Shah, Ganesh Venkataraman"
date: 2024-07-14
venue: "The 47th International ACM SIGIR Conference on Research and Development in Information Retrieval (SIGIR)"
paperurl:
citation:
---
Embedding-based retrieval in graph-based recommendation has shown great improvements over traditional graph walk retrieval methods, and has been adopted in large-scale industry applications such as friend recommendations. However, it is not without its challenges: retraining graph embeddings frequently due to changing data is slow and costly, and producing high recall of approximate nearest neighbor search (ANN) on such embeddings is challenging due to the power law distribution of the indexed users. In this work, we address theses issues by introducing a simple query expansion method in ANN, called FriendSeedSelection, where for each node query, we construct a set of 1-hop embeddings and run ANN search. We highlight our approach does not require any model-level tuning, and is inferred from the data at test-time. This design choice effectively enables our recommendation system to adapt to the changing graph distribution without frequent heavy model retraining. We also discuss how we design our system to efficiently construct such queries online to support 10k+ QPS. For friend recommendation, our method shows improvements of recall, and 11% relative friend reciprocated communication metric gains, now serving over 800 million monthly active users at Snapchat.

[Download paper here](https://github.com/zariable/zariable.github.io/blob/master/files/sirip_2024.pdf)