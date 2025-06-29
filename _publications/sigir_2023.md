---
title: "Embedding Based Retrieval in Friend Recommendation."
collection: publications
permalink: /publication/sigir_2023
excerpt: "Jiahui Shi, Vivek Chaurasiya, Yozen Liu, Shubham Vij, Yan Wu, Satya Kanduri, Neil Shab, Peicheng Yu, Nik Srivastava, Lei Shi, Ganesh Venkataraman, and Jun Yu"
date: 2023-01-01
venue: "Proceedings of the 46th International ACM SIGIR Conference on Research and Development in Information Retrieval (SIGIR)"
paperurl:
citation:
---
Friend recommendation systems in online social and professional networks such as Snapchat helps users find friends and build connections, leading to better user engagement and retention. Traditional friend recommendation systems take advantage of the principle of locality and use graph traversal to retrieve friend candidates, e.g. Friends-of-Friends (FoF). While this approach has been adopted and shown efficacy in companies with large online networks such as Linkedin and Facebook, it suffers several challenges: (i) discrete graph traversal offers limited reach in cold-start settings, (ii) it is expensive and infeasible in realtime settings beyond 1 or 2 hop requests owing to latency constraints, and (iii) it cannot well-capture the complexity of graph topology or connection strengths, forcing one to resort to other mechanisms to rank and find top-$K$ candidates. In this paper, we proposed a new Embedding Based Retrieval (EBR) system for retrieving friend candidates, which complements the traditional FoF retrieval by retrieving candidates beyond 2-hop, and providing a natural way to rank FoF candidates. Through online A/B test, we observe statistically significant improvements in the number of friendships made with EBR as an additional retrieval source in both low- and high-density network markets. Our contributions in this work include deploying a novel retrieval system to a large-scale friend recommendation system at Snapchat, generating embeddings for billions of users using Graph Neural Networks, and building EBR infrastructure in production to support Snapchat scale. 

[Download paper here](https://github.com/zariable/zariable.github.io/blob/master/files/sirip_2023.pdf)