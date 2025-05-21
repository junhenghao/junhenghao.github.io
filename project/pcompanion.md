---
layout: default
title: P-Companion - A principled framework for diversified complementary product recommendation
---

# P-Companion: A principled framework for diversified complementary product recommendation

## Abstract

If one customer [Pablo Alborán](https://www.pabloalboran.es/) buys a tennis racket, what are the best 3 complementary products to purchase together? 3 tennis ball packs, 3 headbands, 3 overgrips, or 1 of each respectively? Complementary product recommendation (CPR), aiming at providing product suggestions that are often bought together to serve a joint demand, forms a pivotal component of e-commerce service, however, existing methods are far from optimal. Given one product, how to recommend its complementary products of different types is the key problem we tackle in this work. We first conduct an extensive analysis to correct the inaccurate assumptions adopted by existing work to show that co-purchased products are not always complementary and further propose a new strategy to generate clean distant supervision labels for CPR modeling. Moreover, to bridge in the gap from existing work that CPR does not only need relevance modeling but also requires diversity to fulfill the whole purchase demand, we develop a deep learning framework, P-Companion to explicitly model both relevance and diversity. More specifically, given one product with its product type, P-Companion first uses an encoder-decoder network to predict multiple complementary product types, then a transfer metric learning network is developed to project the embedding of query product to each predicted complementary product type subspace and further learn the complementary relationship based on the distant supervision labels within each subspace. The whole framework can be trained from end-to-end and robust to cold-start products attributed to a novel pretrained product embedding module named Product2Vec, based on graph attention networks. Extensive offline experiments show that P-Companion outperforms state-of-the-art baselines by 7.1% increase on the Hit@10 score with well-controlled diversity. Production-wise, we deploy P-Companion to provide online recommendations for over 200M products at Amazon and observe significant gains on product sales and profit.

## Modeling

{{< figure library="true" src="project/p-companion.png" title="Workflow of Product Companion: Diversified Complementary Product Recommendation. *P-Companion* has three major components: *Product2vec Embedding module* (encoding all products with their features to pre-trained embeddings), *Type Transition Module* (modeling the mapping function from one type to its complementary types) and *Item Prediction Module* (predicting corresponding items given the query product with associated complementary product types)." lightbox="true">}}

## More Info

**Publication:** The 29th ACM International Conference on Information and Knowledge Management (CIKM 2020)

**Date:** October, 2020

**Links:** [ACM Library](https://dl.acm.org/doi/10.1145/3340531.3412732), [PDF](/assets/files/pubs/CIKM20_PCompanion.pdf), [Video](https://drive.google.com/file/d/1Q-9WvNu_UkP6t-FeO3JtE1qRCqVkxfbH/view?usp=sharing), [Slides](/assets/files/pubs/CIKM20-PCompanion-slides-shot.pdf), [Amazon Science Blog](https://www.amazon.science/blog/improving-complementary-product-recommendations). 