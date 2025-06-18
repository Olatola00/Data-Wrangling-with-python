# Dog Breeds Data Analysis

<a id="#intro"></a>
# Introduction
This repository contains the Python code and analysis for a personal project focused on the intricate processes of data wrangling, cleaning, and exploratory data analysis (EDA) of dog breed information. The goal of this project was to tackle real-world messy data, implement robust cleaning techniques, and then derive initial insights to understand trends and characteristics within the dataset.

This project serves as a practical demonstration of essential data preparation skills, highlighting the importance of data quality before any meaningful analysis can be performed.

**Motivation/Problem Statement:** Real-world data is messy, and this project demonstrates robust techniques to clean and prepare it for analysis. Howeever, project was carried out as part of the requirement to complete the data analyst nanodegree course on Udacity.

**Objectives:** The 3 major objectives of this project are to: 
1. Gather dog data from different sources in different file formats. 
2. Clean the data in preparation for analysis. 
3. Uncover basic insights about dog breeds in the data.

**Methodology/Key Technologies:** Python, Pandas, NumPy, Matplotlib, Seaborn, Requests, Tweepy, JSON parsing, Regular Expressions, Data Merging, Data Type Conversion, Handling Missing Data, Reshaping Data (wide to long).

**Key Findings/Insights**
1. The most common dog breed is a retriever, whether Golden or Labrador.
2. The most loved dog breed by @WeRateDogs’ twitter followers is a little Great Pyrenees.
3. The most rated Dog breed is a Border collie that loves ice cream.


<a href="#data"></a>
## The Data
The main dataset is the tweet archive of a Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. You can read more about them [here](). WeRateDogs mailed the data to the Udacity team as a **csv** file exclusively for use in this project. The archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017.

An additional data was scraped from the **Twitter's API** using the *tweepy* library on Python. This data was required to get the number of likes (**favorite_count**) and retweets (**retweet_count**) each @WeRateDogs' tweets get since they were not included in the Twitter archive.

Finally, additional data on dog breed predictions was provided as a **tsv** file by the Udacity's team. This data was generated after matching each dog's image through a [neural network](https://www.youtube.com/watch?v=2-Ol7ZB0MmU) that classifies breeds of dogs (although this is beyond the scope of this project, you can learn more about how this was done on Udacity's [Machine Learning Engineer Nanodegree course](https://www.udacity.com/course/machine-learning-engineer-nanodegree--nd009)).


## File Structure Explanation: 

- `README.md`: This file, providing an overview of the project, motivation, methodology, key findings, and file structure.
- `wrangle_act.ipynb`: The Jupyter Notebook containing the detailed data gathering, assessing, cleaning, and analysis process.
- `visualize_act.ipynb`: This Jupyter Notebook dedicated for visualizations)
- `twitter_archive_enhanced.csv`: The primary dataset containing WeRateDogs tweet data.
- `twitter_master.csv`: The final, cleaned, and merged dataset ready for further analysis.
- `image-prediction.tsv`: The dataset containing dog breed predictions from the neural network.
- `tweet_json.txt`: The raw JSON data scraped from the Twitter API.

---

**Contact Information/Acknowledgement:** Oladotun Oguntola, [www.linkedin.com/in/oladotun-oguntola-a72715105](www.linkedin.com/in/oladotun-oguntola-a72715105).
