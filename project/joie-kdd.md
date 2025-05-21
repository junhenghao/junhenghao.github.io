---
layout: default
title: Knowledge Graph Embedding on Instances and Ontological Concepts
---

# Knowledge Graph Embedding on Instances and Ontological Concepts

## Abstract

Many large-scale knowledge bases simultaneously represent two views of knowledge graphs (KGs): an ontology view for abstract and commonsense concepts, and an instance view for specific entities that are instantiated from ontological concepts. Existing KG embedding models merely focus on representing one of the two views alone. However, simultaneous learning from both views will likely produce better knowledge embedding models and enable new applications that rely on multi-view knowledge. In this paper, we propose a novel two-view KG embedding model, JOIE. JOIE employs both cross-view and intra-view models that learn on multiple facets of the knowledge base. The cross-view association model is learned to bridge between the embeddings of ontological concepts and their corresponding instance-view entities. The intra-view models are trained to capture the structured knowledge of instance and ontology views in separate embedding spaces, with a hierarchy-aware encoding technique enabled for ontologies with latent hierarchies. We explore multiple representation techniques for the two model components and investigate with nine variants of JOIE. Our model is trained on large-scale knowledge bases that consist of massive instances and their corresponding ontological concepts connected via a (small) set of cross-view links. Experimental results on public datasets show that the best variant of JOIE significantly outperforms previous models on instance-view triple prediction task as well as ontology population on ontology-view KG. In addition, our model successfully extends the use of KG embeddings to entity typing with promising performance.

## Modeling

<!-- {{< figure library="true" src="/assets/img/project/kdd19-joie-twoview.png" title="Fig 1: An example of two-view KB. Regular metarelations and hierarchical meta-relations are denoted as orange and black dashed lines respectively in the ontology view." lightbox="true">}} -->
<img src="/assets/img/project/kdd19-joie-twoview.png" alt="Fig 1: An example of two-view KB. Regular metarelations and hierarchical meta-relations are denoted as orange and black dashed lines respectively in the ontology view." style="display: block; margin-left: auto; margin-right: auto;">

## More Info

**Publication:** The 25th International ACM SIGKDD Conference on Knowledge Discovery and Data Mining (KDD 2019)

**Date:** August, 2019

**Links:** [Paper (ACM Library)](https://dl.acm.org/citation.cfm?id=3330838), [PDF](/assets/files/pubs/KDD19-JOIE.pdf), [Github](https://github.com/JunhengH/joie-kdd19), [Video](https://youtu.be/krJP6Lpa4so), [Slides](/assets/files/pubs/KDD19-JOIE-Presentation.pdf), [Poster](/assets/files/pubs/KDD19-JOIE-Poster.pdf)

