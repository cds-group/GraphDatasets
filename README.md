## GraphDatasets

## On Whole Graph Embedding Techniques

Graph datasets and links to software used in [1], for the evaluation of whole graph embedding techniques for graph classification.

### Data description

#### Synthetic datasets
1. LFR networks: <br /> The [LFR.zip](GraphData/Synthetic/LFR.zip) dataset was generated in [3], using the Lancichinetti–Fortunato–Radicchi (LFR) benchmark method with mixing parameters (μ) 0.1 and 0.5. Originally downloaded from https://github.com/leoguti85/GraphEmbs.<br />
#classes = 2,  #graphs = 1600 (600 with 0.1μ - class1 and 1000 with 0.5μ - class2),  #nodes = 81.
	
2. MREG networks: <br />
The [MREG.zip](GraphData/Synthetic/MREG.zip) was generated using the Multiple Random Eigen Graphs (MREG) model defined in [4].<br />
#classes = 3,  #graphs = 300 (100 in each class, graphJE_1 to 100 - class1, graph_JE101 to 200 - class2 and graph_JE201 to 300 - class2),  #nodes = 100
   
#### Real-world datasets
1. Kidney Metabolic networks:<br />
The [KidneyMetabolic.zip](GraphData/Real/KidneyMetabolic.zip) file contains metabolic networks of 299 Kidney cancer samples (TCGA-KIRC and TCGA-KIRP) [2].<br />
#classes = 3,  #graphs = 299 (159 clear cell Renal Cell Carcinoma - class1, 90 Papillary Renal Cell Carcinoma - class2 and  50 solid tissue normal samples - class3),  #nodes = 1034.

2. Brain fMRI networks:<br />
The [BrainfMRI.zip](GraphData/Real/BrainfMRI.zip) file contains 124 brain fMRI networks of healthy control and schizophrenia subjects.
In this dataset, the edges between the nodes represent the positively correlated brain regions. For both positively and negtively correlated edges please visit the original source of this dataset: https://github.com/jesusdaniel/graphclass, where the authors provide an R package along with the COBRE dataset.<br />
#classes = 2,  #graphs = 124 (70 controls - class1 and 54 schizophrenia subjects - class2),  #nodes = 263.

#### Sample annotation
The  [DataAnnotation](DataAnnotation) folder contains the sample annotations and graph class labels for all the four datasets.

### Links to software

1. Distribution-based graph distance measures: https://github.com/cds-group/GraphDistances [2]
2. Autoencoder: https://github.com/leoguti85/GraphEmbs [3]
3. JointEmbedding (Matrix factorization): https://github.com/jesusdaniel/JEG [4]
4. Graph Kernels:<br />
   Weisfeiler-lehman optimal assignment kernel: https://nl.mathworks.com/matlabcentral/fileexchange/64711-weisfeiler-lehman-optimal-assignment-kernel [5]<br />
   Shortest path kernel: https://www.dbs.ifi.lmu.de/~borgward/papers/BorKri05.pdf [6]<br />
   Random walk kernel: https://www.jmlr.org/papers/volume11/vishwanathan10a/vishwanathan10a.pdf [7]<br />

### References
[1] Maddalena, L., Manipur, I., Manzo, M. and Guarracino, M.R., 2020, November. On Whole-Graph Embedding Techniques. In International Symposium on Mathematical and Computational Biology (pp. 115-131). Springer, Cham.
https://link.springer.com/chapter/10.1007/978-3-030-73241-7_8

[2] Granata, I., Guarracino, M.R., Kalyagin, V.A., Maddalena, L., Manipur, I. and Pardalos, P.M., 2020. Model simplification for supervised classification of metabolic networks. Annals of Mathematics and Artificial Intelligence, 88(1), pp.91-104.
https://link.springer.com/article/10.1007/s10472-019-09640-y

[3] Gutiérrez-Gómez, L. and Delvenne, J.C., 2019. Unsupervised network embeddings with node identity awareness. Applied Network Science, 4(1), p.82. https://link.springer.com/article/10.1007/s41109-019-0197-1

[4] Wang, S., Arroyo, J., Vogelstein, J.T. and Priebe, C.E., 2019. Joint embedding of graphs. IEEE Transactions on Pattern Analysis and Machine Intelligence. https://ieeexplore.ieee.org/abstract/document/8889404

[5] Kriege, N.M., Giscard, P.L. and Wilson, R., 2016. On valid optimal assignment kernels and applications to graph classification. In Advances in Neural Information Processing Systems (pp. 1623-1631). https://papers.nips.cc/paper/6166-on-valid-optimal-assignment-kernels-and-applications-to-graph-classification.pdf

[6] Borgwardt, K.M. and Kriegel, H.P., 2005, November. Shortest-path kernels on graphs. In Fifth IEEE international conference on data mining (ICDM'05) (pp. 8-pp). IEEE. https://www.dbs.ifi.lmu.de/~borgward/papers/BorKri05.pdf

[7] Vishwanathan, S.V.N., Schraudolph, N.N., Kondor, R. and Borgwardt, K.M., 2010. Graph kernels. The Journal of Machine Learning Research, 11, pp.1201-1242. https://www.jmlr.org/papers/volume11/vishwanathan10a/vishwanathan10a.pdf

#### <sup>**</sup>For more graph related work visit our github page at [cds-group](https://github.com/cds-group/)
