# Clustering_Project
## Brief Description 
For this project I've taken on the hypothetical role as a consultant for a company's marketing department. The client is interested in forming a marketing strategy for a new product and wants to determine what customers would be most receptive to their product. The data provided for this task includes customer id's and credit card data such as balance, purchases, purchase freq, etc. I decided to use a clustering algorithm to determine groups of customers based on their purchase behaviors and disposable income. A client/staholders could leverage these clusters of potential customers to influence their marketing outreach strategy or compose an A/B test on selected clusters of interest.

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
- Standardize features 
- Train model using a Euclidean Distance Matrix
- Determine optimal no. of clusters using elbow method
- Create and cut a dendrogram at the optimal no. of clusters
- Visualize Clusters using cluster package
- Use group_by to aggregate data by cluster and compare/contrast average attribute values for each cluster
- Full analysis of each cluster and what product/service would be most well suited for these clusters of customers

## Why is this useful?
The results of this project can prove incredibly useful to any company who wishes to determine what consumer target groups are ideal for a product/service of interest. Of course, companies could take this data and without machine learning simply market to consumers that meet certain thresholds (> 100,000 balance, > 50 purchases a month, etc.). However, with clustering there is less guessing about how large or narrow a target group should be or how thresholds should be determined. As mentioned in the "Characerizing clusters" portion of `Clustering_project.Rmd`, if there are certain thresholds stakeholders are interested these clusters can be narrowed down by removing outliers. 

What I found most ineresting about this project was that I could vaguely determine the demographics of the clusters based only on banking data. Of course some of these demographic descriptors are derived from generalizations, such as, younger people have less money and make frequent purchases. This could be very useful for a company who is targetting new customers and doesn't have suitable demographic data. However, it would be wise to spend the extra money for demographic data and merge with the banking data to vastly improve the results of our clustering algorithm. 

If intersted in reading my full analysis and observing source code please follow the instructions under "How to run this project."
