# Text mining project 
## Checking the alignment of global actions and development targets
### Ivan Vallejo Vall, 19 June 2017

The code used to generate the figures and charts included in the final report is divided into three Jupyter notebooks written in Python 2.7. They are stored in the Box folder "source_code". They should be run in sequential order, as indicated below. 

As an alternative, the file "intermediate_inputs.zip" includes the ".csv" outputs of running the respective notebooks. Unzipping this file in the same directory as the Jupyter notebooks allows to run the notebooks in any order. I would propose to unzip this file in any case, and then run the code. There is no harm in overwritting and this ensures that you can run all the code even when skipping some of the longest processing operations (i.e. the complete web scraping of the ITU website -- may take 15-30 minutes).

**Important:** the files "goal4.txt", "goal5.txt", "goal9.txt", "goal14.txt" and "goal17.txt" are needed as an input to create the dictionaries. They are contained in the file "intermediate_inputs.zip" and should be unzipped in the same directory as the Jupyter notebooks *before executing the second notebook*.   

Currently, the Jupyter notebooks output the charts inline, although it is indicated when relevant how to output the result into a file. If you scrape again the ITU website (rather than using the results of my scraping), please consider that, there might minor variations in some charts, as some of the content on the ITU website may have changed. 

Each code chunk in the Jupyter notebooks contains an explanation of the requirements (i.e. python libraries to be imported), inputs and outputs. I ran it in an AWS instance and did not have problems installing the python packages using pip (it should also work with anaconda or any other python environment manager). In my computer, it took me a little more time because I am using a virtual environment (to separate py2 and py3) and the packages did not always get installed in the virtual environment.

Note: the Jupyter notebooks do not include any explanation on the results and the rationale for the chosen methodologies. This information is available on the project report.     


**List of Jupyter notebooks:**

1. "scrape.ipynb": Web scraping of the links and text content on the ITU website (www.itu.int). Outputs the file "ITU_links_text.csv" which is required to run Jupyter notebook 3.

2. "dictionaries.ipynb": Creation of dictionaries for SDGs 4, 5, 9, 14 and 17. Requires the corresponding .txt files in the same directory to execute the first code chunk. Outputs the file "dictionaries.csv" which is required to run Jupyter notebook 3.

3. "analysis.ipynb": Creates the charts and figures that address the research question: is the content on the ITU website aligned with the Sustainable Development Goals?