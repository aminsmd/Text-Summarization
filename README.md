# Text-Summarization

> Text summarization is a process of shortening a text document in a way that it contains the main points of the original document.

### How can summarization help us?
* reduces reading time
* lorem ipsum
* lorem ipsum

### There are two main approaches in text summarization:
* Extraction: When the sentences of the summary are selected from the original document.
* Abstraction: When the model creates new sentences and forms a summary. Humans summarize documents mostly based on abstractive method.

### Based on purpose
* Generic: Model tries to make a general summary of the document and treats all inputs the same.
* Query-Based: Model summarizes based on a natural language question.

### Based on input type
* Single Document: Model creates the summary based on 1 paper or document.
* Multiple Document: Model generates the summary based on multiple papers about a specific subject.

## Our approach

### TextRank algorithm
The main idea in this approach is to find sentence embeddings by averaging vector representations of the words of sentence and assign the cosine similarity of those vectors to weights of a fully connected graph. Then perform a pagerank algorithm on this graph and chose the sentences with higher rank as the sentences of our extractive summary.
