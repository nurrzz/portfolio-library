# Project Library

Python used to be my favorite programming language. Back in college, I taught it in the computer lab, and I’ve also built with Django. These days I work with ASP.NET, but apparently old favorites still get a few weekends.

This library is where those experiments go. The first one starts with a simple question: how much of a Netflix catalog snapshot is made up of movies, and how much is TV shows?

## Projects

| Project | Research question | Tools |
| --- | --- | --- |
| [Netflix Catalog Analysis](projects/netflix-catalog-analysis/analysis.ipynb) | What share of the Netflix catalog snapshot consists of movies and TV shows? | Python, KaggleHub, Google Colab |

## Netflix Catalog Analysis

### Project objective

This case study measures the mix of movies and TV shows in a Netflix catalog snapshot. A content team could use this breakdown as a baseline before comparing the mix across release decades.

### Dataset

The analysis uses the [Netflix Movies and TV Shows dataset on Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows). Each row represents a listing. The notebook previews the listing ID, title, and content type before using the type field to calculate the breakdown.

### Method

1. Download the dataset with KaggleHub and preview five rows to check the fields used in the analysis.
2. Read the CSV with Python’s `csv` module and count the listings labeled `Movie` or `TV Show`.
3. Divide each count by the combined movie and TV show count to calculate its share.

### Output and scope

The notebook prints a count and percentage for each category and identifies which category makes up the larger share. A TV series counts as one listing regardless of its number of seasons. The figures describe the listings in this dataset. Questions about viewing behavior would require audience data.

### Reproduce the analysis

Download the [notebook](projects/netflix-catalog-analysis/analysis.ipynb), open it in Google Colab, and run the cells in order. The notebook installs KaggleHub, downloads the dataset, and calculates the results.

## In progress

More Python and data projects are in progress and will be added as they’re completed.
