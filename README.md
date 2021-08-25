# Subjective Answer Finder &nbsp;[![](https://img.shields.io/badge/python-3.8.5-blue.svg)](https://www.python.org/downloads/) [![platform](https://img.shields.io/badge/platform-JupyterNB-red.svg)](https://github.com/Viral-Doshi/Auto-Answering-NLP) 


## Objectives:<br>
* Keyword Extraction: To get keywords which best define the document<br>
* Summarization: to generate paragraph-wise Summaries of the document<br>
* Creating a NLP model which generates automatic subjective answers using Information Retrieval and Summarization techniques<br>


## Model Architecture:<br>
![image](https://github.com/Viral-Doshi/Auto-Answering-NLP/blob/main/arch.png)

## Methodology and Work-Flow:<br>
* Step 1:  Raw Text Data to Organized DataFrame
* Step 2:  Paragraph-wise Keyword Extraction
* Step 3:  Vectorizing Keywords to form Representative Vectors for paragraphs
* Step 4:  Summarizing Paragraphs to generate fixed length Answers
* Step 5:  Query Question to Vector
* Step 6:  Scoring Function to calculate Paragraph Scores
* Step 7:  Selecting Best Answer based on Final Scores

## Source Code:
* [This file](https://github.com/Viral-Doshi/Auto-Answering-NLP/blob/main/Step1%20Analysis.ipynb) has Analysis and Visualizations of the text document we are working with.
* [This file](https://github.com/Viral-Doshi/Auto-Answering-NLP/blob/main/Step2%20Keywords_Extraction_Ch2.ipynb) contains the Paragraph-wise Keyword Extraction using 6 different methods.
* [This file](https://github.com/Viral-Doshi/Auto-Answering-NLP/blob/main/Step3%20Paragraph-Wise%20Summarization.ipynb) contains the Paragraph-wise Summarization using 5 different methods
* [This file](https://github.com/Viral-Doshi/Auto-Answering-NLP/blob/main/Auto-Answering.ipynb) is the final implementation of Subjective Answer Finder. The last cell contains a small GUI-like interface.

## Requirements
* Please install the required dependancies.
* Download glove encodings from [here](https://www.kaggle.com/danielwillgeorge/glove6b100dtxt) and place it in the same directory.
* Text format of my document is as follows:
  * Chapter Name on the first line followed by a blank line.
  * Paragraph-title followed by the paragraph description.
  * A empty line after completion of each paragraph.
  * 2 empty lines at the end of chapter before the Question/Answer section.

## Conclusion:<br>
* This method can be used effectively for Information Retrieval purposes for obtaining relevant information from big text documents
* This Auto-Answering Model can also be used to find subjective answers to given Questions from Textbooks
* Accuracy ~ 75% ( Spacy + Model1)
* Many NLP based tasks such as Keyword Extraction, Vectorization and Summarization are performed which has many individual applications
