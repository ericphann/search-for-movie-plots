# Homework 3: Search for Movie Plots 📽️  
## What's included?
- 3 notebooks
  1. [semantic search](https://github.com/ericphann/search-for-movie-plots/blob/main/notebooks/01-semantic_search.ipynb)
  2. [reranker](https://github.com/ericphann/search-for-movie-plots/blob/main/notebooks/02-reranker.ipynb)
  3. [RAG](https://github.com/ericphann/search-for-movie-plots/blob/main/notebooks/03-rag.ipynb)
- executive analysis writeup [ [pdf](https://github.com/ericphann/search-for-movie-plots/blob/main/writeups/Analysis%20Writeup.pdf) | [docx](https://github.com/ericphann/search-for-movie-plots/blob/main/writeups/Analysis%20Writeup.docx) ]
- [requirements.txt](https://github.com/ericphann/search-for-movie-plots/blob/main/requirements.txt)
## Objective
Develop a prototype for a search tool that helps users find relevant movies based on their queries.
## Dataset
Use the following code to import the [dataset](https://www.kaggle.com/datasets/jrobischon/wikipedia-movie-plots?resource=download), if needed.

    from datasets import load_dataset  
    ds = load_dataset("Coder-Dragon/wikipedia-movies", split='train[:1000]')

The dataset includes movie titles, plots, genres, actors, and some other information regarding movies. For this experiment we will only focus on the first 1,000 movies, which are _movies from the 1920s or earlier_. We will also only focus on querying and embedding the titles and plots.
## Usage
You should be able to run the notebooks in Colab seamlessly. If there are dependency-related errors or if you'd like to run the notebooks locally, you can use the included [requirements.txt](https://github.com/ericphann/search-for-movie-plots/blob/main/requirements.txt).  

The recommendation is to run the notebooks in the following order: semantic search, then reranker, then RAG. This is because this follows the order they were completed in and because they build in complexity. Evaluation metrics are calculated in the notebooks where applicable.  

Finally, feel free to review the executive analysis writeup for experiment findings and recommendations. An appendix is included with all experiment metrics and results neatly organized into tables. 
