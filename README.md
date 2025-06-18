# Dog Breeds Data Analysis

## Table of Contents
<ul>
<li><a href="#intro">Introduction</a>
    <ul><a href="#data">The Datasets</a></ul>
</li>
<li><a href="#wrangling">Data Wrangling</a>
    <ul><a href="#gather">Data Gathering</a></ul>
    <ul><a href="#assess">Data Assessment</a></ul>
    <ul><a href="#clean">Data Cleaning</a></ul>
</li>
    
<li><a href="#viz">Data Visualization and Analysis</a></li>
<li><a href="#conclusions">Conclusion</a></li>
</ul>

<a id="#intro"></a>
# Introduction

Dogs are the only mammal on earth having the most variable number of breeds. The [Fédération Cynologique Internationale (FCI)](https://www.hillspet.com/dog-care/behavior-appearance/how-many-dog-breeds-are-there) lists about 360 breeds globally, the **Labrador retriever** being the most popular of them all based on a rating by the [American Kennel Club](https://www.akc.org/most-popular-breeds/) in 2021.

As part of the requirement to complete the data analyst nanodegree course on Udacity, this data wrangling project was carried out on various dog data.

The 3 major objectives of this project are to: 
1. Gather dog data from different sources in different file formats. 
2. Clean the data in preparation for analysis. 
3. Uncover basic insights about dog breeds in the data.


<a href="#data"></a>
## The Data
The main dataset is the tweet archive of a Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. You can read more about them [here]().

This data was emailed to the Udacity team by WeRateDogs as a **csv** file exclusively for use in this project. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017.


The first additional data was scraped from the **Twitter's API** using the *tweepy* library on Python. This data was required to get the number of likes (**favorite_count**) and retweets (**retweet_count**) each @WeRateDogs' tweets get since they were not included in the Twitter archive.

The last additional data was generated from the Twitter archive after each image in the archive was ran through a [neural network](https://www.youtube.com/watch?v=2-Ol7ZB0MmU) that can classify breeds of dogs (although this is beyond the scope of this project, you can learn more about how this was done on Udacity's [Machine Learning Engineer Nanodegree course](https://www.udacity.com/course/machine-learning-engineer-nanodegree--nd009)). The result was provided as **tsv** files available for download on Udacity's website.
