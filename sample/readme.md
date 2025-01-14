1. The **create_index.py** gives the index number to each lncRNA, microRNA and disease in the heterogeneous tripartite network.

2. The **deepwalk_training.py** generates the feature vector for each biomedical node in the tripartite network.

3. The **rule_based_prediction.py** calculates the association score for each lncRNA-disease pair.

4. The **PMC_hits.py** and **Pubmed_hits.py** are used for prediction result validation on [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/) 
and [PubMed Center](https://www.ncbi.nlm.nih.gov/pmc/)(PMC). They are designed as multi-thread parallel programs.

5. The rest of **deep_walk_training_CV.py**, **prediction_CV.py** and **parallel_prediction_CV.py** are for 5-fold cross validation (CV). The **parallel_prediction_CV.py** is multi-process programmed.

The codes were written and tested using [Pandas](https://pandas.pydata.org/) version 0.23. For the data index manner in Pandas has changed from `.ix[,]` to `.loc[,]` or `iloc[,]` since version 1.0.0, please replace `.ix[,]`s by `.loc[,]`s or degrade your Pandas version if your are using Pandas>=1.0.0.  
