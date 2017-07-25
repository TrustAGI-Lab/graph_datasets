# graph_dataset

This repository maintains several benchmark graph datasets, which are widely used for graph classification. The graph datasets ranges from chemical compounds, scientific publications, to twitter sentiment graphs. The chemical compound graph datasets are in “.sdf” or “.smi” format, and other graph dataset are represented as “.nel” format. All these graph datasets can be handle by frequent subgraph miner packages such as Moss [1] and other softwares. 

1.	NIC Anti-cancer activity prediction data (NCI)
Description: 
The NCI graph datasets are commonly used as the benchmark for graph classification. Each NCI dataset belongs to a bioassay task for anticancer activity prediction, where each chemical compound is represented as a graph, with atoms representing nodes and bonds as edges. A chemical compound is positive if it is active against the corresponding cancer, or negative otherwise. 
Number of Dataset: 18 (9 balanced dataset + 9 imbalanced dataset)


2.	PTC Predictive Toxicology Challenge Data (PTC)
Description: 
This PTC graph dataset include a number of carcinogenicity tasks for toxicology prediction of chemical compounds.

The dataset we selected contains 417 compounds from four types of test animals: MM (male mouse), FM (female mouse), MR (male rat), and FR (female rat). Each compound is with one label selected from {CE, SE, P, E, EE, IS, NE, N}, which stands for Clear Evidence of Carcinogenic Activity (CE), Some Evidence of Carcinogenic Activity (SE), Positive (P), Equivocal (E), Equivocal Evidence of Carcinogenic Activity (EE), Inadequate Study of Carcinogenic Activity (IS), No Evidence of Carcinogenic Activity (NE), and Negative (N).
Number of Dataset:  8 (4 + 4)



3.	DBLP Graph Datasets (DBLP)
Description:
The DBLP dataset consists of bibliography data in computer science. Each record in DBLP is associated with a number of attributes such as abstract, authors, year, venue, title, and reference ID. To build a graph stream, we select a list of conferences (as shown in Table I) and use the papers published in these conferences (in chronological order) to form a binary-class graph stream. The classification task is to predict whether a paper belongs to DBDM (database and data mining) or CVPR (computer vision and pattern recognition) field, by using the references and the title of each paper. 
Number of Dataset: 1



4.	Twitter Sentiment Graph Data
Description:
This dataset is extracted from twitter sentiment classification. Because of the inherently short and sparse nature, twitter sentiment analysis (i.e., predicting whether a tweet reflects a positive or a negative feeling) is a difficult task. To build a graph dataset, we represent each tweet as a graph by using tweet content, with nodes in each graph denoting the terms and/or smiley symbols (e.g, :-D and :-P) and edges indicating the co-occurrence relationship between two words or symbols in each tweet. To ensure the quality of the graph, we only use tweets containing 20 or more words. We select the tweets from April 6 to June 16 to generate 140,949 graphs (in a chronological order). This dataset has been used for graph stream classification in [3] and cost-sensitive learning in [2].
Number of Dataset: 1


5.	Functional Brain Network Analysis Data
Description:
BrainNet Functional Brain Network Analysis Data are constructed from the whole brain functional magnetic res- onance image (fMRI) atlas [6]. The purpose of the study is to map brain as a network (or a graph) where each node corresponds to a region of Interest (ROI) and the edge indicates correlations between two ROIs. In our experiments, we use functional parcellation results, CC200, from [6], which parcellate each brain into 200 regions of interest. In order to discover relationships between ROIs, the mean values of each ROI are recorded with respect to certain voxel time courses. By using Pearson correlations between two time courses, we can calculate correlation between two ROIs, and a graph is constructed by connecting ROIs whose correlations is higher than a threshold value. For ADHD and HI tasks, the functional response is real values, so we discretize the functional response to binary values by using a simple threshold. 
Number of Dataset: 3

