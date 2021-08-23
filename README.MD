# Reading List of Homophily (Assortative) in GNNs
Homophily is an important staticticis for network estimation, which indicates the consistency of labeling information and structural information (e.g., 1-hop neighborhood, adjacency matrix). On the contrary, heterophily is to depict the disconsistency of those information. Besides, assortative and disassortative are the synonyms for homophily and heterophily. 

Originally, the idea of homophily is derived from social network, with strongly grounded explanation that similar people are more likely to make connections. [Video of homophily in social network](href="https://www.youtube.com/watch?v=x5d8FPpcSdI")

In recent years, the idea of homophily began to be explored in graph neural networks. It is a good point that more and more attention has been paid into the ralationships of the attributes of the networks themselves and the propagation mechanisms. Usually, homophily is taken as a prior assumption as the success of GNNs, demonstrated by the impressive performance on citation networks (e.g., cora, citeseer and pubmed) with high homophily. In the other hand, benchmarks with high heterophily are causing enmergerging interest to evaluate the effectiveness of a GNN model more comprehensively. 

To sum up, this repository is made to provide a *reading list of relative (basically) conference papers about homophily (heterophily) in GNNs*, where **two tracks** are separated: 
- &#10004; Modeling improvements 
- &#10008; Analysis and discussions 
  
| Title | Year | Conference | Descriptions | Type |
| :---- | :--: | :--------: | :---         | :--: |
| [Graph Neural Networks with Heterophily](href="https://arxiv.org/abs/2009.13566") | 2021 | AAAI | Propose a model called CPGNN that utilizes compatibility matrix to filter the signal from the compatible classes in every propagation step. | &#10004; |
| [Beyond Homophily in Graph Neural Networks: Current Limitations and Effective Designs](href="https://arxiv.org/abs/2006.11468") | 2020 | NeurIPS | Propose H2GCN to flatten and maintain all the information that a network could provide. Three operations are adopted: ego- and neighbor- embedding seperation, higher-order neighborhoods and combination of intermediate representations. | &#10004; |
| [Is Homophily a Necessity for Graph Neural Networks?](href="https://arxiv.org/abs/2106.06134") | 2021 | Arxiv | Designing experiments to indicate that homophily is not important to GNNs, and with fine-grid hyperparameters turning, GCN works well on heterophily datasets. | &#10008; |
| [Non-Local Graph Neural Networks](href="https://arxiv.org/abs/2005.14612") | 2020 | Arxiv | Targeting at disassortive graph, it designs various non-local aggregation in GNN. | &#10004; |

# TODO
Summary of benchmarks

