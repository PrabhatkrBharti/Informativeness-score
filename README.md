# <div align="center"> A Method for Automatically Estimating the Informativeness of Peer Reviews</div>
This repository contains dataset and code of the "A Method for Automatically Estimating the \textit{Informativeness} of Peer Reviews" Authors: Prabhat Kumar Bharti, Tirthankar Ghoshal, Mayank Agrawal, Asif Ekbal, Affiliation: Indian Institute of Technology, Patna, India


------

### Folders in main repository:

- **[annotated_reviews_dataset](https://github.com/pripat-2002/Review_Informativeness/tree/main/annotated_reviews_dataset) :** <br />
    - contains the [Annotated_Review_18 zip file](https://github.com/pripat-2002/Review_Informativeness/blob/main/annotated_reviews_dataset/Annotated_Review_18-20220806T163727Z-001.zip), which is a dataset of text files containing 1323 annotated reviews from the ICLR 2018 Conference, that was used for making the Gold-standard Informativeness Score Formula.
    - contains the [reviews_csv csv file](https://github.com/pripat-2002/Review_Informativeness/blob/main/annotated_reviews_dataset/reviews_csv.csv), which is a dataset containing the paper meta decision, review decision and confidence scores of the ICLR 2018 reviews used; included in case of use in future work.
  
  
- **[baseline_res](https://github.com/pripat-2002/Review_Informativeness/tree/main/baseline_res) :**<br />
    - contains the output csv files from the baseline ICLR 2018 reviews analysis.<br />
    
- **[qualitative_res](https://github.com/pripat-2002/Review_Informativeness/tree/main/qualitative_res) :**<br />
    - contains the output csv files from the qualitative ICLR 2018 reviews analysis.<br />
  
- **[graphs](https://github.com/pripat-2002/C_N_reviews/tree/main/graphs) :**<br />
    - contains the graphs and other pictorial charts obtained from the reviews analysis.<br />
    
------

### Files in main repository:

- **[01_init ipynb notebook](https://github.com/pripat-2002/Review_Informativeness/blob/main/Golden_Informativeness_Score_01_init.ipynb) :**<br />
  - contains the codes for initialising the Baseline ICLR 2018 analysis; extracting the annotated labels, finding their coverage and distribution and hence, calculating the Section Scores and Aspect Scores; and also finding features such as "sentence count", "word count", "avg. sentence length", "avg. word length", "vocab length", "hedge word count", "non-hedge word count", and "hedge ratio", for use in future work.<br />

- **[02_hedge ipynb notebook](https://github.com/pripat-2002/Review_Informativeness/blob/main/Golden_Informativeness_Score_02_hedge.ipynb) :**<br />
  - contains the codes for finding the Hedge Score using Tirthankar Ghoshal HedgePeer Model for the baseline ICLR 2018 analysis.<br />

- **[03_fin ipynb notebook](https://github.com/pripat-2002/Review_Informativeness/blob/main/Golden_Informativeness_Score_03_fin.ipynb) :**<br />
  - contains the codes for calculating the Informativeness Score for baseline ICLR 2018 analysis, along with a few other features such as "VADER compound sentiment" and "POS features" for future work.<br />
  
- **[04_Qualitative ipynb notebook](https://github.com/pripat-2002/Review_Informativeness/blob/main/Golden_Informativeness_Score_04_Qualitative.ipynb) :**<br />
  - contains the codes for performing Qualitative Analysis on NIPS 2018 reviews, by extracting their labels, finding all the previously mentioned features, and calculating the Section Score, Aspect Score, Hedge Score and hence, the Informativeness Score..
  
- **[weights json](https://github.com/pripat-2002/Review_Informativeness/blob/main/weights.json) :**<br />
  - contains the weights for each Section and Aspect label obtained from their frequency distribution of overall coverage in all papers, that will be used to calculate the Section and Aspect Scores.

------
