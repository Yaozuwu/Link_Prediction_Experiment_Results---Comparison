# Link Prediction: Experiment Results on Benchmark Datasets

In this repository, We used the medical dataset [DRKG](<https://github.com/gnn4dr/DRKG>) to compare the results of recently published and well-aged approaches to link prediction problems. These methods can be classified into different groups (Classification methods from:[Link-Prediction-Experiment-Results](https://github.com/irokin/Link-Prediction-Experiment-Results)).

1. Rule-based Methods
2. Embedding Methods
3. Graph Neural Network Methods
4. Hybird Methods (relational reinforcement learning, differentiable reasoning, etc.)



#### Type Markers:

- **E** as embedding methods
- **R** as rule-based methods
- **NN** as graph neural nets
- Hybird Methods:
  - **E+NN**
  - **R+NN**
  - **R+E**
  - **R+E+NN**
  - **R+RL** : Rule + reinforcement learning

Approach Format:

**(Approach Type)-(Method Name)-(Published Year)**





##### Dataset:

Drug Repurposing Knowledge Graph (DRKG) is a comprehensive biological knowledge graph relating genes, compounds, diseases, biological processes, side effects and symptoms. DRKG includes information from six existing databases including DrugBank, Hetionet, GNBR, String, IntAct and DGIdb, and data collected from recent publications particularly related to Covid19. It includes 97,238 entities belonging to 13 entity-types; and 5,874,261 triplets belonging to 107 edge-types. These 107 edge-types show a type of interaction between one of the 17 entity-type pairs (multiple types of interactions are possible between the same entity-pair), as depicted in the figure below. It also includes a bunch of notebooks about how to explore and analysis the DRKG using statistical methodologies or using machine learning methodologies such as knowledge graph embedding.



##### Methods:

**Embedding methods:**

- **E**-TransE-2013
  - [Bordes, A., Usunier, N., Weston, J., & Yakhnenko, O. (2013). Translating Embeddings for Modeling Multi-Relational Data. NIPS, 2787–2795.](<https://doi.org/10.1007/s13398-014-0173-7.2>)
  - 
- **E**-DistMult-2015
  - [Yang, B., Yih, W., He, X., Gao, J., & Deng, L. (2015). Embedding entities and relations for learning and inference in knowledge bases. ICLR, 1–13.](<https://arxiv.org/pdf/1412.6575.pdf>)
  - 
- **E**-ANALOGY-2017
  - [Liu, H., Wu, Y., & Yang, Y. (2017). Analogical Inference for Multi-relational Embeddings. ICML.](<http://proceedings.mlr.press/v70/liu17d.html>)
- **E**-SimpleE-2018
  - [Kazemi, S. M., & Poole, D. (2018). SimplE Embedding for Link Prediction in Knowledge Graphs. NIPS, 1–12.](<https://papers.nips.cc/paper/7682-simple-embedding-for-link-prediction-in-knowledge-graphs>)
  - 
- **E**-ConvE-2018
  - [Dettmers, T., Minervini, P., Stenetorp, P., & Riedel, S. (2018). Convolutional 2D Knowledge Graph Embeddings. AAAI, 1811–1818.](<https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/17366>)
  - 
- **E**-ComplEx-N3-2018
  - [Lacroix, T., Usunier, N., & Obozinski, G. (2018). Canonical Tensor Decomposition for Knowledge Base Completion. ICML.](<http://proceedings.mlr.press/v80/lacroix18a.html>)
  - 
- **E**-CrossE-2019
  - [Zhang, W., Paudel, B., Zhang, W., Bernstein, A., & Chen, H. (2019). Interaction Embeddings for Prediction and Explanation in Knowledge Graphs. WSDM.](<https://arxiv.org/pdf/1903.04750.pdf>)
  - 
- **E**-Rotate-2019
  - [Sun, Z., Deng, Z., Nie, J., & Tang, J. (2019). Rotate: Knowledge graph embedding by relational rotation in complex space. ICLR, 1–18.](<https://openreview.net/forum?id=HkgEQnRqYQ>)
  - 
- **E**-IterE-2019
  - [Zhang, W., Paudel, B., Wang, L., Chen, J., Zhu, H., Zhang, W., … Chen, H. (2019). Iteratively Learning Embeddings and Rules for Knowledge Graph Reasoning.](<https://arxiv.org/abs/1903.08948>)
  - 
  
- **E**-Eigenvalue factorization algorithm-
  - [Yamanishi Y, Araki M, Gutteridge A, et al. Prediction of drug–target interaction networks from the integration of chemical and genomic spaces. Bioinformatics 2008;24: i232–40.](<https://doi.org/10.1093/bioinformatics/btn162>)
  -
  - [Yamanishi Y, Kotera M, Moriya Y, et al. DINIES: drug–target interaction network inference engine based on supervised analysis. Nucleic Acids Res 2014;42:W39–45.](<https://doi.org/10.1093/nar/gku337>)
  -
- **E**-Probabilistic matrix factorization-2013
  - [Cobanoglu MC, Liu C, Hu F, et al. Predicting drug–target interactions using probabilisticmatrix factorization.J Chem Inf Model 2013;53:3399–409.](<https://pubs.acs.org/doi/pdf/10.1021/ci400219z>)
  -
- **E**-Matrix factorization-
  - [Zheng X, Ding H, Mamitsuka H, Zhu S. Collaborative matrix factorization with multiple similarities for predicting drug–target interactions. In: Proceedings of the 19th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining—KDD ’13, 2013, pp. 1025–1033. Chicago, Illinois, USA.](<https://dl.acm.org/doi/abs/10.1145/2487575.2487670>)
  -
  - [Ezzat A, Zhao P,WuM, et al. Drug–target interaction prediction with graph regularized matrix factorization. IEEE/ACM Trans Comput Biol Bioinform 2017;14:646–56.](<https://ieeexplore.ieee.org/abstract/document/7407341>)
  -
  - [Shen Z, Zhang Y-H, Han K, et al. miRNA-disease association prediction with collaborative matrix factorization. Complexity 2017;2017:1–9.](<https://www.hindawi.com/journals/complexity/2017/2498957/>)
  -
  - [Zeng X, Ding N, Rodríguez-Patón A, Zou Q. Probability-based collaborative filtering model for predicting gene–disease associations. BMC Med Genomics 2017;10(5):76.](<https://link.springer.com/article/10.1186/s12920-017-0313-y>)
  -
- **E**-LE, SVD, PLS-2017
  - [Ezzat A, Wu M, Li X-L, et al. Drug–target interaction prediction using ensemble learning and dimensionality reduction. Methods 2017;129:81–8.](<https://doi.org/10.1016/j.ymeth.2017.05.016>)
  -
 - **E**-DCA-
  - [Luo Y, Zhao X, Zhou J, et al. A network integration approach for drug–target interaction prediction and computational drug repositioning from heterogeneous information. Nat Commun 2017;8:573.](<https://www.nature.com/articles/s41467-017-00680-8>)
  -
 - **E**-DeepWalk-
  - [Zong N, Kim H, Ngo V, et al. Deep mining heterogeneous networks of biomedical linked data to predict novel drug–target associations. Bioinformatics 2017;33:2337–44.](<https://doi.org/10.1093/bioinformatics/btx160>)
  -
  - [Li G, Luo J, Xiao Q, et al. Predicting microRNA-disease associations using network topological similarity based on DeepWalk. IEEE Access 2017;5:24032–9.](<https://ieeexplore.ieee.org/abstract/document/8085107>)
  -
 - **E**-Modified DeepWalk-2017
  - [Alshahrani M, Khan MA,Maddouri O, et al. Neuro-symbolic representation learning on biological knowledge graphs. Bioinformatics 2017;33:2723–30.](<https://doi.org/10.1093/bioinformatics/btx275>)
  -

 - **E**-Eigenvalue decomposition and matrix factorization-2015
  - [DaiW, Liu X, Gao Y, et al. Matrix factorization-based prediction of novel drug indications by integrating genomic space. Comput Math Methods Med 2015;2015:275045.](<https://www.hindawi.com/journals/cmmm/2015/275045/>)
  -
  
 - **E**-Modified LINE-2017
  - [Wang P, Hao T, Yan J, et al. Large-scale extraction of drug–disease pairs from the medical literature. J Assoc Inf Sci Technol 2017;68:2649–61.](<https://doi.org/10.1002/asi.23876>)
  -
- **E**-Extended RESCAL-2016
  - [Zitnik M, Zupan B. Collective pairwise classification for multi-way analysis of disease and drug data. Pac Symp Biocomput 2016;21:81–92.](<https://doi.org/10.1142/9789814749411_0008>)
  -
- **E**-TransH and HolE-2017
  - [Abdelaziz I, Fokoue A, Hassanzadeh O, et al. Large-scale structural and textual similarity-based mining of knowledge graph to predict drug–drug interactions. Web Semant 2017;44:104–17.](<https://doi.org/10.1016/j.websem.2017.06.002>)
  -
 
- **E**-Extended TransH-2017
  - [Wang M, Chen Y, Qian B, et al. Predicting rich drug–drug interactions via biomedical knowledge graphs and text jointly embedding, 2017, arXiv preprint arXiv:171208875.](<https://arxiv.org/abs/1712.08875>)
  -
 
- **E**-Isomap-2010
  - [You Z-H, Lei Y-K, Gui J, et al. Using manifold embedding for assessing and predicting protein interactions from high-throughput experimental data. Bioinformatics 2010;26:2744–51](<https://doi.org/10.1093/bioinformatics/btq510>)
  -

  
  
**Rule-based methods:**

- **R**-Node+LinkFeat-2015
  - [Toutanova, K., & Chen, D. (2015). Observed versus latent features for knowledge base and text inference. Proceedings of the 3rd Workshop on Continuous Vector Space Models and Their Compositionality, 57–66.](<https://doi.org/10.18653/v1/w15-4007>)
  - 
- **R**-AMIE-2015
  - [Galárraga, L., Teflioudi, C., Hose, K., & Suchanek, F. M. (2015). Fast rule mining in ontological knowledge bases with AMIE+. VLDB Journal, 24(6), 707–730.](<https://doi.org/10.1007/s00778-015-0394-1>)
  - 
- **R**-Gaifman-2016
  - [Niepert, M. (2016). Discriminative gaifman models. NIPS, 3413–3421.](<https://papers.nips.cc/paper/6098-discriminative-gaifman-models>)
  - 
- **R**-RuleN-2018
  - [Meilicke, C., Fink, M., Wang, Y., Ruffinelli, D., Gemulla, R., & Stuckenschmidt, H. (2018). Fine-grained evaluation of rule- and embedding-based systems for knowledge graph completion. ISWC, 3–20.]( <https://doi.org/10.1007/978-3-030-00671-6_1>)
  - 
- **R**-RUGE-2018
  - [Guo, S., Wang, Q., Wang, L., Wang, B., & Guo, L. (2018). Knowledge Graph Embedding with Iterative Guidance from Soft Rules. AAAI, 4816–4823.](<https://arxiv.org/abs/1711.11231>)
  - 
- **R**-AnyBURL-2019
  - [Meilicke, C., Chekol, M. W., Ruffinelli, D., & Stuckenschmidt, H. (2019). Anytime Bottom-Up Rule Learning for Knowledge Graph Completion. IJCAI, 3137–3143.](<https://www.ijcai.org/Proceedings/2019/435>)
  - 

**Graph neural nets:**

- **NN**-R-GCN-2017
  - [Kipf, T. N., & Welling, M. (2017). Semi-Supervised Classification with Graph Convolutional Networks. ICLR, 1–14.]( <http://arxiv.org/abs/1609.02907>)
  - 
- **NN**-SACN-2019
  - [Shang, C., Tang, Y., Huang, J., Bi, J., He, X., & Zhou, B. (2019). End-to-End Structure-Aware Convolutional Networks for Knowledge Base Completion. AAAI, 3060–3067.](<https://aaai.org/ojs/index.php/AAAI/article/view/4164>)
  - 
- **NN**-Deep autoencoder similar to SDNE and DNGR-2018
  - [Zitnik M, Agrawal M, Leskovec J. Modeling polypharmacy side effects with graph convolutional networks. Bioinformatics 2018. doi:10.1101/258814](<https://doi.org/10.1093/bioinformatics/bty294>)
  -

**Hybird Methods:**

- **R+E**-RLvLR-2018
  - [Omran, P. G., Wang, K., & Wang, Z. (2018). Scalable rule learning via learning representation. IJCAI, 2149–2155.](<https://arxiv.org/abs/1911.08935>)
  - 
- **R+E**-RPJE-2020
  - [Niu, G., Zhang, Y., Li, B., Cui, P., Liu, S., Li, J., & Zhang, X. (2020). Rule-Guided Compositional Representation Learning on Knowledge Graphs. AAAI.](<https://arxiv.org/abs/1911.08935>)
  - 
- **E+NN**-R-GCN+-2018
  - [Schlichtkrull, M., Kipf, T. N., Bloem, P., Titov, I., & Welling, M. (2018). Modeling Relational Data with Graph Convolutional Networks. ESWC, 593–607.](<https://arxiv.org/abs/1703.06103>)
  - 
- **E+NN**-ConvKB-2018
  - [Nguyen, D. Q., Nguyen, T. D., Nguyen, D. Q., & Phung, D. (2018). A Novel Embedding Model for Knowledge Base Completion. NAACL.](<https://arxiv.org/abs/1712.02121>)
  - 
- **E+NN**-AttentionE-2019
  - [Nathani, D., Chauhan, J., Sharma, C., & Kaul, M. (2019). Learning Attention-based Embeddings for Relation Prediction in Knowledge Graphs. ACL.](<http://arxiv.org/abs/1906.01195>)
  - 
- **R+NN**-Neural LP-2017
  - [Yang, F., & Cohen, W. W. (2017). Differentiable Learning of Logical Rules for Knowledge Base Reasoning. NIPS.](<https://papers.nips.cc/paper/6826-differentiable-learning-of-logical-rules-for-knowledge-base-reasoning.pdf>)
  - 
- **R+NN**-NTP lambda-2017
  - [Rocktäschel, T., & Riedel, S. (2017). End-to-End Differentiable Proving. NIPS.](<http://arxiv.org/abs/1705.11040>)
  - 
- **R+NN**-DRUM-2019
  - [Sadeghian, A., Armandpour, M., Ding, P., & Wang, D. Z. (2019). DRUM: End-To-End Differentiable Rule Mining On Knowledge Graphs. NIPS, 1–13.](<http://arxiv.org/abs/1911.00055>)
  - 
- **R+RL**-MINERVA-2018
  - [Das, R., Dhuliawala, S., Zaheer, M., Vilnis, L., Durugkar, I., Krishnamurthy, A., … Mccallum, A. (2018). Go for a walk and arrive at the answer: Reasoning over paths in knowledge bases using reinforcement learning. ICLR.](<https://arxiv.org/pdf/1711.05851.pdf>)
  - 
- **R+RL**-Multi-Hop-2018
  - [Lin, X. V., Richard, S., & Caiming, X. (2018). Multi-Hop Knowledge Graph Reasoning with Reward Shaping. ACL, 3243–3253.](<https://www.aclweb.org/anthology/D18-1362/>)
  - 





