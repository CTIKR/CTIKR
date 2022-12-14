# CTIKR

## Introduction
CTIKR(Cyber Threat Intelligence Knowledge Representation) is a tool to extract knowledge from open source CTI articles. It uses a sentence classification NLP model to identify sentences that are related to cyber attacks from article, then clusters the articles based on the sentences. Meanwhile, it extracts knowledge graphs from the sentences.

For a given article as the input, CTKIR can extract the following information: the most important sentences that describe attack's behavior and the tactics they used, the Cyber attack tactics included in the article, the graph of attack behavior, the cluster of the article. Based on those article information, CTKIR achieved the following applications on large scale articles: Entity Behavior Discovery, Topic Classification, Attack Campaign Discovery, Kill Chain Summary.

## Overview
CTIKR contains three main components. The overview figure is shown below.

![image](https://i.imgur.com/J0dFYWv.png)

1.[Knowledge Extraction](https://github.com/CTIKR/CTIKR/tree/main/Knowledge%20Extraction): Automatic extraction of cyber threat knowledge. CTIKR has a knowledge base of CTI sentences based on existing cyber threat knowledge bases two machine learning models to identify the sentences.

2.[Knowledge Representationn](https://github.com/CTIKR/CTIKR/tree/main/Knowledge%20Representation): Construction of article clusters and knowledge graph based on extracted knowledge.

3.[Knowledge Discovery](https://github.com/CTIKR/CTIKR/tree/main/Knowledge%20Discovery): Four security applications based knowledge discovery of the cyber threat knowledge threat knowledge.  

## Tool Requirements
Python Version >= 3.8.0

Python Library:

numpy >= 1.23.4

scikit-learn >= 1.1.2

simpletransformers >= 0.63.9

hdbscan >= 0.8.28

torch >= 1.12.1

networkx >= 2.8.7

cdlib >= 0.2.6
