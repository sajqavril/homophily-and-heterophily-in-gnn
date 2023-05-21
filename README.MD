# A Reading List of Homophily (Assortative) in GNNs
Homophily is an important staticticis for network estimation, which indicates the consistency of labeling information and structural information (e.g., 1-hop neighborhood, adjacency matrix). On the contrary, heterophily is to depict the disconsistency of those information. Besides, assortative and disassortative are the synonyms for homophily and heterophily. 

Originally, the idea of homophily is derived from social network, with strongly grounded explanation that similar people are more likely to make connections. [This is a video of homophily in social network.](https://www.youtube.com/watch?v=x5d8FPpcSdI)

In recent years, the idea of homophily began to be explored in graph neural networks. It is a good point that more and more attention has been paid into the ralationships of the attributes of the networks themselves and the propagation mechanisms. Usually, homophily is taken as a prior assumption as the success of GNNs, demonstrated by the impressive performance on citation networks (e.g., cora, citeseer and pubmed) with high homophily. On the other hand, benchmarks with high heterophily are causing enmergerging interest to evaluate the effectiveness of a GNN model more comprehensively. 

To sum up, this repository is made to provide a *reading list of relative (basically) conference papers about homophily (heterophily) in GNNs*, where **two tracks** are separated: 
- &#10004; Model improvements 
- &#10008; Analysis and discussions 
  
| ID | Title | Year | Conference | Descriptions | Type | Group |
| :--: | :---- | :--: | :--------: | :---         | :--: | :--: |
| :one: | [Graph Neural Networks with Heterophily](https://arxiv.org/abs/2009.13566) | 2021 | AAAI | It proposes a model called CPGNN that utilizes compatibility matrix to filter the signal from the compatible classes in every propagation step. | &#10004; | Danai Koutra (University of Michigan) |
| :two: | [Beyond Homophily in Graph Neural Networks: Current Limitations and Effective Designs](https://arxiv.org/abs/2006.11468) | 2020 | NeurIPS | It proposes H2GCN to flatten and maintain all the information that a network could provide. Three operations are adopted: ego- and neighbor- embedding seperation, higher-order neighborhoods and combination of intermediate representations. | &#10004; | Danai Koutra (University of Michigan) |
| :three: | [Is Homophily a Necessity for Graph Neural Networks?](https://arxiv.org/abs/2106.06134) | 2021 | Arxiv | Designing experiments to indicate that homophily is not important to GNNs, and with fine-grid hyperparameters turning, GCN works well on heterophily datasets. | &#10008; | Jiliang Tang (Michigan State University) |
| :four: | [Non-Local Graph Neural Networks](https://arxiv.org/abs/2005.14612) | 2020 | Arxiv | Targeting at disassortive graph, it designs various non-local aggregation operations on GNNs. | &#10004; | Shuiwang Ji (Texas A&M University) |
| :five: | [Two Sides of the Same Coin: Heterophily and Oversmoothing in Graph Convolutional Neural Networks](https://arxiv.org/abs/2102.06462) | 2021 | Arxiv | It gives a unified framework to analyze *over-smoothing* and *heterophily* simultaneously. And the modeling novelty is a signed function for neighborhood aggregation, a filter by favoring the similar ones (similar to :one:). | &#10008; &#10004; | Danai Koutra (University of Michigan) |
| :six: | [Improving Robustness of Graph Neural Networks with Heterophily-Inspired Designs](https://arxiv.org/abs/2106.07767) | 2021 | Arxiv | It attributes the sensitivity of GNNs to the homophily assumption that impactful structral attacks leads to increased heterophily. The improvements are similar to :two:. | &#10004; | Danai Koutra (University of Michigan) |
| :seven: | [Energy Levels Based Graph Neural Networks for Heterophily](https://iopscience.iop.org/article/10.1088/1742-6596/1948/1/012042/meta) | 2021 | Journal of Physics: Conference Series | On the base of :two:, it proposes an energy function based model to distinguish other classes besides itself, while :two: treats them equaly. | &#10004; | Youfa Liu (Huazhong Agricultural University) |
| :eight: | [GCN-SL: Graph Convolutional Networks with Structure Learning for Graphs under Heterophily](https://arxiv.org/abs/2105.13795) | 2021 | Arxiv | It proposes two operations: one is efficient aggregation of similar nodes avoiding long-range aggregation, the other is re-connected adjacency based on node similarity. | &#10004; | Xinliang Wu (Xi’an Jiaotong University) |
| :nine: | [Unifying Homophily and Heterophily Network Transformation via Motifs](https://arxiv.org/abs/2012.11400) | 2021 | Arxiv | It proposes a plugin to encode higher-order proximity under both homophily and heterophily conditions via a random-walking method. All the baselines are random-walking approaches. | &#10004; | Haiping Lu (University of Sheffield) |
| :one::zero: | [Label Propagation on K-Partite Graphs with Heterophily](https://ieeexplore.ieee.org/abstract/document/8812910) | 2021 | TKDE | In both heterogenous and heterophily graph, it proposes a novel label propagation algorithm. | &#10004; | Linhong Zhu (Univ. of Southern California) |
| :one::one: | [Geom-GCN: Geometric Graph Convolutional Networks](https://openreview.net/forum?id=S1e2agrFvS) | 2020 | ICLR | Well-cited datasets. | &#10004; | Bo Yang (Jilin University) |
| :one::two: | [New Benchmarks for Learning on Non-Homophilous Graphs](https://arxiv.org/abs/2104.01404) | 2021 | WWW | It presents a series of improved graph datasets with node label relationships that do not satisfy the homophily principle, with new measure approches. | &#10008; | Cornell University & Facebook AI |
| :one::three: | [On the Equivalence between Positional Node Embeddings and Structural Graph Representations](https://arxiv.org/abs/1910.00452) | 2020 | ICLR | Very interesting points on the relation between node feature and graph structure, implying the effectiveness of homophily performing as clustering in node classification task. | &#10008; | Perdue University |
| :one::four: | [Improving Your Graph Neural Networks: A High-Frequency Booster](https://arxiv.org/abs/2210.08251) | 2022 | ICDMW | It propose a high-pass regularizer for GNNs, with theoretical proofs. | &#10008; &#10004; | Tsinghua University |
| :one::five: | [Feature Extension for Graph Neural Networks](https://arxiv.org/pdf/2305.06142.pdf) | 2023 | ICML | It propose an novel feature space view for analyzing GNNs, with rigorous theoretical adjustifications and convincing experimental results. | &#10008; &#10004; | Tsinghua University |




# Heterophilic benchmarks
:star: - recommended objectively

- [OGB](https://ogb.stanford.edu/docs/nodeprop/): the heterophilic ones are included in the two links below. 
- :star: [Cornell-University-AI/Non-Homophily-Benchmarks](https://github.com/CUAI/Non-Homophily-Benchmarks/tree/main/data)
- :star: [Cornell-University-AI/Non-Homophily-Large-Scale](https://github.com/CUAI/Non-Homophily-Large-Scale)
- :star: [torch-geometric.datasets](https://pytorch-geometric.readthedocs.io/en/latest/modules/datasets.html#torch_geometric.datasets.Amazon):the rest of all the heterophilic datasets can all be found here, with nice descriptions and citation information, e.g., actor/chameleon/squirrel/film.

