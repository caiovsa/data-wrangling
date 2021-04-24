# Data Wrangling Project

<p align="center">
  <img src="https://camo.githubusercontent.com/95e20f5a43f022791ea4580765c3b2bb5d0583525d4c635e68caa12bbf03f212/68747470733a2f2f64313768323774366835313561352e636c6f756466726f6e742e6e65742f746f706865722f323031372f4f63746f6265722f35396464333738665f646f672d72617465732d736f6369616c2f646f672d72617465732d736f6369616c2e6a7067" width="925" title="hover text">
</p>

# Introduction
 This was one of the projects from the Udacity Data Analyst nanodegree, where the student was given the task to gather data from the twitter account WeRateDogs. The twitter account like the name suggests, rates dogs in a funny way, so people send their dogs pictures so they give a review about them, of course in the end all of them get very high grades (like 14/10, 10/10) because of course, all dogs are really cute.

 The student needed to gather the data from a lot of sources, clean it, and use this data to make a single dataset with all the data in the best shape for a simple and quick analysis in the end, and to show some of my skills too.

# Process
### Gathering the Data
In the project, we gathered our data from three different sources, using three different methods to gather it.
1. The first dataset was given by Udacity in a CSV file, so we just needed to download and read it. This first dataset was the tweets history from the account WeRateDogs, given by them.
2. The second, was hosted on the Udacity servers, so it should be downloaded programmatically. This one is a dataset with the tweets image predictions (Given by a Neural Network), so this dataset give us a prediction of the dog breed (or object sometime) in the image that was tweeted.
3. The last one that we used, was gathered using the twitter API (Tweepy library in python) and saving each tweet's returned JSON as a new line in a .txt file. We used the same tweet id from the first dataset, so we could get the last infos needed (Like retweets count) to complement the first part.

### Assessing the Data
During the notebook i made some observations about the datasets, and i took notes with the details that im changing in them (Cleaning step). I divided them in Quality and Tidiness problems.

### Cleaning the data
The last step that i took was of course, clean the data! And in the end i merged them into one single dataframe, with all the necessary features and some problems adjusted.
I saved it in a csv and database file.

### Analysis
After all that i realized some small analysis, checking things like: Breed popularity, Dog types and some others

# Files
* twitter_archive_master.csv ---> The full dataset, with all the info needed;

* doggo_archive.db ---> Full dataset, stored on a sqlite database;

* image_predictions.tsv ---> File downloaded from Udacity servers, it contains the image predictions from the tweets (given by a Neural Net);
 
* tweet_json.txt ---> Where we stored the data gathered from the API;

* twitter-archive-enhanced.csv ---> First dataset, with the tweets from WeRateDogs;
 
* Wrangle_act.ipynb ---> Jupyter notebook file.
