# job-cv-matching
This is a Python notebook with the core functionality of an application that finds the best matching CV's for a given job posting. It uses openai's GPT-models for interpreting and transforming CV documents. It is a useful tools for finding the best candidates for a position among a large number of possible choices. This can help save valuable time for bid managers and similar professions.

The process outline is this:
1. Get CV documents from CV database
2. Summarize the CV documents to make them shorter and more information dense
3. Transform the CV documents to numerical embeddings in order to compare them with job postings in an easy way
4. Read a job posting and transform it in the same way as with the CV documents
5. Compare the job posting with all the CV documents and find the best matches
6. Present the names and rankings of the found matches

## Pre-requisites
- In order to run this notebook you will need access to a suitable dataset of CV documents. If you have a [Kaggle](https://www.kaggle.com/) account you can download and use the same dataset as i have used in this notebook. More information in the relevant section of the notebook.
- You will also need a deployment of two GPT-models. One for text summarization and one for text embedding. The easiest way to set this up is to deploy an openai-resource on a Microsoft Azure subscription. Microsofts documentation will help you to set up the required accounts and resources. Once you have that in place, you will be able to retrieve an openai endpoint adress along with an access key that you can insert in the relevant section of this notebook.
