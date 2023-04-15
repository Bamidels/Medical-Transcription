# Medical-Transcription
Medical Transcription Information Extraction
This is a project that aims to extract useful information from medical transcriptions using natural language processing (NLP) techniques. The dataset used in this project is available on Kaggle and can be downloaded from https://www.kaggle.com/datasets/tboyle10/medicaltranscriptions?resource=download 
Dependencies
Aim
The aim of this project is to extract useful information from medical transcriptions. Specifically, the project requires extracting the sex and age information of patients, as well as the treatment that they received from the transcription column. The project instructions also encourage exploring different ways in which treatment information can be expressed in the transcription column and developing algorithms to catch them. 

The following dependencies are required to run this project:

pandas
numpy
re
transformers
torch
seaborn
matplotlib
scikit-learn

We performed the task testing several models that:

Extracts the sex and age information of each patient from the transcription text using regular expressions
Extracts the treatment information of each patient from the transcription text using the BioBERT model, BioBert_NN, and a model of Bert with a different tokenizer and model from the Hugging Face Transformers library
I also tried some KMeans clustering on the encoded sex, age, and treatment information of each patient
Computes cluster statistics, including the mean age and the most common treatment for each cluster
I also attempt to train a GP-2 model on the data for extracting treatment information from the medical transcriptions. 

proposed ourput
BioBert for treatment extraction: The output of this model is a string representing the treatment information extracted from the medical transcription.

Hugging Face Transformers' DialoGPT-small for clustering: The output of this model is a set of cluster statistics, including the mean age and most common treatment for each cluster.

BioBert for classification: The output of this model is a set of predicted labels for a given set of input data.
