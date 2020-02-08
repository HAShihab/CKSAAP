Predicting the Effects of Amino Acid Substitutions using K-Spaced Amino Acid Pairs
----

## Description

The Composition of K-Spaced Amino Acid Pairs (CKSAAP) has been used to predict a number of different sites in protein sequences, including:

Site|Paper
-|-
Flexible / Rigid Regions|[Chen, K., Kurgan, L.A. & Ruan, J. Prediction of flexible/rigid regions from protein sequences using k-spaced amino acid pairs.](https://bmcstructbiol.biomedcentral.com/articles/10.1186/1472-6807-7-25)
Palmitoylation Sites|[Xiao-Bo Wang, Ling-Yun Wu, Yong-Cui Wang, Nai-Yang Deng. Prediction of palmitoylation sites using the composition of k-spaced amino acid pairs.](https://academic.oup.com/peds/article/22/11/707/1485136)
Phosphorylation Sites|[Zhao X, Zhang W, Xu X, Ma Z, Yin M. Prediction of Protein Phosphorylation Sites by Using the Composition of k-Spaced Amino Acid Pairs.](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0046302)
Ubiquitination Sites|[Chen, Zhen & Zhou, Yuan & Song, Jiangning & Zhang, Ziding. HCKSAAP-UbSite: Improved prediction of human ubiquitination sites by exploiting amino acid pattern and properties.](https://www.sciencedirect.com/science/article/abs/pii/S157096391300160X)
Lysine Formylation|[Ju, Zhe & Wang, Shi-Yun. Prediction of lysine formylation sites using the composition of k-spaced amino acid pairs via Chou's 5-steps rule and general pseudo components](https://www.sciencedirect.com/science/article/pii/S0888754319302198)

In summary, the scheme constructs a sequence fragment of 2n + 1 around the site of interest, using n upstream residues and n downstream residues, and calculates the number of k-spaced amino acid pairs observed.  For all values of k, there are 400 different combinations of amino acid pairs (i.e. 20 x 20).  The only difference between the k-spaced amino acid pairs is the number of residues that seperate the pairs.  For example:

k|k-Spaced Amino Acid Pairs|No. of Combinations
-|-|-
0|AA, AC, AD, …, AY|400
1|AxA, AxC, AxD, …, AxY|400
2|AxxA, AxxC, AxxD, …, AxxY|400

where x can be any one of the 20 possible any amino acids.

This project applies CKSAAP to predict the effects of amino acid substitutions.  A sequence fragment of 21 is constructed, i.e. 10 upstream and 10 downstream residues from the site of interest, and k-spaced amino acid pairs with k = 0, 1, …, 5 is used. 

## License

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)

**Free Software, Hell Yeah!**