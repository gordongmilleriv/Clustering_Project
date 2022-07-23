# Clustering_Project
## Brief Description 
For this project I've taken on the hypothetical role as a consultant for a company's marketing department. The client is interested in forming a marketing strategy for a new product and wants to determine what customers would be most receptive to their product. The data provided for this task includes customer id's and credit card data such as balance, purchases, purchase freq, etc. I decided to use a clustering algorithm to define groups of customers whom are most likely to buy this new product. Purchase likelihood is determined by factors such as disposable income, purchase frequency, bank balance, etc. 

## How to run this project
1. Download `Clustering_project.Rmd` Markdown file
2. Download the provided csv data file: `ccdata.csv`
3. Download `lab_templet.css` in the same folder as `ccdata.csv` - used for formatting Rmd file
4. Open R.Studio and download required packages
5. Open and knit `Clustering_project.Rmd` as html in R.Studio 
6. After initiating the knit select `ccdata.csv` from your file directory when prompted to choose a file to upload

## Required Packages
- caret
- cluster
- reshape2
- tidyverse
- corrplot
- gridExtra
- factoextra
- kableExtra
- here

## What does this project do?
- Replace numeric NA values with mean value for the variable
- Evaluate correlations between features 
- Evaluate outliers
- Standardize features/

## Why is this useful?

