# The Anatomy of a Hit: Statistically Learning from the Best

## Overview

What makes a hit pop song? This paper examines the audio features that characterize mainstream music's biggest hits. This self-directed study utilizes audio feature data from top artists' discographies, accessed through the Spotify API, to analyze via multiple linear regression which specific musical qualities significantly impact a song's assigned popularity score on Spotify.

## File Structure

The repo is structured as:

-   `data/raw_data` contains the raw data as obtained from the Spotify API using spotifyr.
-   `data/analysis_data` contains the cleaned dataset that was constructed.
-   `model` contains fitted models. 
-   `other` contains relevant literature, details about LLM chat interactions, and rough sketches.
-   `paper` contains the files used to generate the paper, including the Quarto document and reference bibliography file, as well as the PDF of the paper. 
-   `scripts` contains the R scripts used to simulate, download and clean data.

## Reproducing Graphs and Tables
Here is a quick guide to reproducing my graphs and tables.

1. Install RStudio or any R language interpreter. Install the libaries indicated in the `setup` chunk at the top.  
2. Go to `paper/paper.qmd`
3. Navigate to any of the R chunks, denoted by {r some-title} (fig denotes a figure, tbl denotes a table)
4. Copy and paste the code into your interpreter and run. 
   
## Statement on LLM usage

Aspects of my R code and paper were written and edited with the assistance of Large Language Models, in particular variants of Claude-3 (Claude.ai) and GPT-4 (ChatGPT). 

Claude-3 Sonnet/Haiku was used for:
- Writing and editing parts of the paper

GPT-4 was used for: 
- Coding some of the R graphs
- Debugging and troubleshooting

The complete chat history with both models are available in inputs/llms. 
