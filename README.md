# Text mining project 
## Checking the alignment of global actions and development targets
### Ivan Vallejo Vall, June 2017

This project uses text mining methods to assess whether the activities of the International Telecommunication Union (ITU) are aligned with the Sustainable Development Goals.

The ITU website was scraped and dictionary methods were applied to each webpage to determine whether the topics covered corresponded to some preselected SDGs. A term frequency–inverse document frequency (TF-IDF) weighting was applied to the corpus of ITU webpages. Specific dictionaries for each SDG were built by applying latent Dirichlet allocation (LDA) to a set of labeled documents characteristic of these topics. 

The results are presented in the PDF document published in this repository. The python source code is included in the folder 'code' organized into three different Jupyter notebooks.   

