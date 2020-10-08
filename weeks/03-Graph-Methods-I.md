---
layout: week
title: Week 03
doodle: /doodle.png
---

# Domain specific techniques I: Intro to GCNs

## Topics

This week's assignments will guide you through the following topics:
* An introduction to Graph Neural Networks
* Build a graph neural network

## Reading

Please read the following:
*[Graph Convolutional Networks](http://tkipf.github.io/graph-convolutional-networks/)
*[Tutorial on Graph Neural Networks for Computer Vision and Beyond](https://medium.com/@BorisAKnyazev/tutorial-on-graph-neural-networks-for-computer-vision-and-beyond-part-1-3d9fada3b80d)
*Read slides 10-44 from the [presentation on GCN and GraphSage](http://snap.stanford.edu/proj/embeddings-www/files/nrltutorial-part2-gnns.pdf)

### Replication task
* Read Section 3 of the [GraphSage]((https://www-cs.stanford.edu/~jure/pubs/graphsage-nips17.pdf),) paper.


## Tasks

Complete the following tasks:
* Run the [full training models]((https://github.com/bknyaz/examples/blob/master/fc_vs_graph_train.py) from the tutorial comparing a fully connected network (FCN), convolutional network (CNN) and graph convolutional network (GCN). Report the results.
* Implement a 1-layer GCN and train it on a node classification task for the Cora dataset. The Cora dataset consists of 2708 scientific publications classified into one of seven classes. The citation network consists of 5429 links. Each publication in the dataset is described by a 0/1-valued word vector indicating the absence/presence of the corresponding word from the dictionary. The dictionary consists of 1433 unique words. The README file in the dataset provides more details.
    [Download Link](https://linqs-data.soe.ucsc.edu/public/lbc/cora.tgz). Compare the performance of the GCN to an FCN and report the results.

## Weekly Questions

Answer the following questions
* In both MNIST and Cora you are training a neural network to perform a clasification task on your samples. However in the two implementations of the GCN, the graph plays a different role. Explain. (hint: who are the features, nodes and edges in each of these tasks).
* Describe one thing that you found difficult to understand in Section 3 of the paper. Try to be specific about what you don’t think you understand.
