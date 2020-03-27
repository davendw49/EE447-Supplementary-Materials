---
layout: post
title:  "Knowledge Graph Material"
date:   2020-03-27 22:39:26 -0700
categories: sc
---

## 论文和相关资料

 - [知识图谱大礼包](http://dataset.acemap.cn/EE447/knowledge-graph.tar.gz)

## 知识图谱技术栈

很多人会认为知识图谱是商家提升自身应用市场影响力的噱头，此话不假。但是从技术本身回看知识图谱的技术栈，我们发现其实涵盖计算机的各种方向的技术应用。

 - 知识数据的采集需要掌握实体抽取和关系抽取的知识，例如命名实体识别和基于远程监督的关系抽取
 - 面对提取的数据需要掌握大规模数据存储的技能，例如分布式数据库和分布式图数据库
 - 面对图数据我们还可以拓展到大规模的网络表示学习或者知识表示学习
 - 面对知识图谱的图结构，我们还可以基于图数据转机器表示，即语言生成
 - 加上本体论为基础的规则逻辑的表示方式，知识图谱初始的语义网技术也是一大模块

可以说知识图谱涵盖人工智能中的符号主义和连接主义的从古至今的大部分应用。

 ![avatar](../../../../supplementary/stack.png)

## 知识图谱的前世今生

相信有相当一部分人已经在各大平台看过很多知识图谱的相关推送了，这边就做一个简单的链接的搬运工，也是网站的站长执笔的三篇推送：

 1. [Acemap研究周报之知识图谱（一）：追根溯源](https://archive.acemap.info/academic-report/knowledge-graph)
 2. [Acemap研究周报之知识图谱（二）：非常建筑](https://archive.acemap.info/academic-report/knowledge-graph2)
 3. [知识图谱系列之回到未来](https://archive.acemap.info/academic-report/knowledge-graph3)

## 目前KG+的研究领域

### NLP

自然语言处理的领域实在是太广阔了下面分享两个资源：

 - [https://github.com/dair-ai/nlp_paper_summaries](https://github.com/dair-ai/nlp_paper_summaries)
 - [Standford NLP网课](https://www.youtube.com/watch?v=OQQ-W_63UgQ&list=PL3FW7Lu3i5Jsnh1rnUwq_TcylNr7EkRe6&index=2&t=0s)

### 图神经网络

作为一个搬运工，知乎上的一个比较认可的回答：

 - GCN(Max Welling那篇)是谱域的GNN,基于谱图理论,无法天然的处理有向图.
 - GAT是空域的GNN可以天然的处理有向图,通常定义入度的节点进行聚合.
 - 至于知识图谱/异质图也有专门设计的GNN.知识图谱上的GNN关注于了对于不同关系含义的区别,
 - 参考: 19KDD KGAT Knowledge Graph Attention Network for Recommendation异质图上的GNN关注于多种不同关系的融合来更好的描述节点

如何将不能天然处理异构有向图的知识图谱和GNN结合起来是一个很热门的领域。像[Text Generation from Knowledge Graphs with Graph Transformers](https://arxiv.org/abs/1904.02342?context=cs)这篇文章把带属性的图转成了不带属性的无向图，并且用graph transformer提取特征。

### 知识表示学习

知识图谱的表示学习自然是很多的，详细可以看清华刘知远老师团队整理的KRL的[Paperlist](https://github.com/thunlp/KRLPapers)

### QA

知识图谱的最直接应用就是QA，问答系统远没有我们想象的好做，小编从本科二年级开始研究KBQA，真心觉得是一个巨坑，有一个小众的[Research Track](https://github.com/SeanLee2Cod/KBQA_Paper)

### 图数据库

知识图谱的存储是一个亟待解决的问题，如果你们的选题设计图数据库，可以直接联系[daven](mailto:davendw@sjtu.edu.cn)

