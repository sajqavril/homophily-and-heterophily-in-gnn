# Reading List of Homophily (Assortative) in GNNs
Homophily is an important staticticis for network estimation, which indicates the consistency of labeling information and structural information (e.g., 1-hop neighborhood, adjacency matrix). On the contrary, heterophily is to depict the disconsistency of those information. Besides, assortative and disassortative are the synonyms for homophily and heterophily. 

Originally, the idea of homophily is derived from social network, with strongly grounded explanation that similar people are more likely to make connections. [This is a video of homophily in social network.](https://www.youtube.com/watch?v=x5d8FPpcSdI)

In recent years, the idea of homophily began to be explored in graph neural networks. It is a good point that more and more attention has been paid into the ralationships of the attributes of the networks themselves and the propagation mechanisms. Usually, homophily is taken as a prior assumption as the success of GNNs, demonstrated by the impressive performance on citation networks (e.g., cora, citeseer and pubmed) with high homophily. On the other hand, benchmarks with high heterophily are causing enmergerging interest to evaluate the effectiveness of a GNN model more comprehensively. 

To sum up, this repository is made to provide a *reading list of relative (basically) conference papers about homophily (heterophily) in GNNs*, where **two tracks** are separated: 
- &#10004; Modeling improvements 
- &#10008; Analysis and discussions 
  
| Title | Year | Conference | Descriptions | Type |
| :---- | :--: | :--------: | :---         | :--: |
| [Graph Neural Networks with Heterophily](https://arxiv.org/abs/2009.13566) | 2021 | AAAI | It proposes a model called CPGNN that utilizes compatibility matrix to filter the signal from the compatible classes in every propagation step. | &#10004; |
| [Beyond Homophily in Graph Neural Networks: Current Limitations and Effective Designs](https://arxiv.org/abs/2006.11468) | 2020 | NeurIPS | It proposes H2GCN to flatten and maintain all the information that a network could provide. Three operations are adopted: ego- and neighbor- embedding seperation, higher-order neighborhoods and combination of intermediate representations. | &#10004; |
| [Is Homophily a Necessity for Graph Neural Networks?](https://arxiv.org/abs/2106.06134) | 2021 | Arxiv | Designing experiments to indicate that homophily is not important to GNNs, and with fine-grid hyperparameters turning, GCN works well on heterophily datasets. | &#10008; |
| [Non-Local Graph Neural Networks](https://arxiv.org/abs/2005.14612) | 2020 | Arxiv | Targeting at disassortive graph, it designs various non-local aggregation operations on GNNs. | &#10004; |
| [Two Sides of the Same Coin: Heterophily and Oversmoothing in Graph Convolutional Neural Networks](https://arxiv.org/abs/2102.06462) | 2021 | Arxiv | ... | &#10008; |
| [Improving Robustness of Graph Neural Networks with Heterophily-Inspired Designs](https://arxiv.org/abs/2106.07767) | 2021 | Arxiv | ... | &#10004; |
| [Energy Levels Based Graph Neural Networks for Heterophily](https://iopscience.iop.org/article/10.1088/1742-6596/1948/1/012042/meta) | 2021 | Journal of Physics: Conference Series | ... | &#10004; |
| [GCN-SL: Graph Convolutional Networks with Structure Learning for Graphs under Heterophily](https://arxiv.org/abs/2105.13795) | 2021 | Arxiv | ... | &#10004; |
| [Unifying Homophily and Heterophily Network Transformation via Motifs](https://arxiv.org/abs/2012.11400) | 2021 | Arxiv | ... | &#10004; |
| [Label Propagation on K-Partite Graphs with Heterophily](https://ieeexplore.ieee.org/abstract/document/8812910) | 2021 | TKDE | ... | &#10004; |


# TODO
Summary of benchmarks

