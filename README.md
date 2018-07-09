# Metis_Bootcamp
Metis Datascience Project 2 - Webscraping & Linear Regresion Modeling

For this project, I utilized beautiful soup to scrape loan information from the Kiva website. I augmented this data through utlizing the publicly available API to download additional loan information for historical Kiva loans. In all, I had a dataset with 1.4 million loans from 92 counties. The loan information was for the years 2006-2018.

With the loan information, I specifically was interested in identifying factors that contributed to the length of time it takes a loan to get funded on Kiva. 98% of all Kiva loans receive full funding, through feature selection could I determine what determines how long it will take a loan to receive funding.

For my initial data exploration I took a subset of 50,000 loans and investigated where the loan requests come from, what industry sector the loans are for, who was seeking loans. I utilized a Box-Cox transformation on some of the data to normalize and scale it, I performed a basic sentiment analysis on the description, and a calculated what percent of the loan seekers were male and female.

After initial data exploration, I focused in on funded loans from Kenya. Kenya receives the second largest number of loans on Kiva and I was interested in what factors played a role there. I utilized a subic polynomial model to try and extract additional information from interaction of various data points. To account for the increased dimensionality from using a cubic polynomial, I also utilized elastic net regularization to only retain a subset of features.

Overall, I found that there is low predictability about the length of time it takes a project to get funded. My model was able to account for approximately 33.5% of the variability in length of time to funding. For more insights and information feel free to explore my jupyter notebooks or view my presentation files for more detailed analysis.

Outdated files are in the archive.
