![Illustration of a Person standing in front of a news article. The news article has grey and yellow text lines. Two modules are connected to those textlines, one stating "biased" (yellow) and one stating "not biased" (grey)](/TeaserImage.png)
# NewsUnfold
This repository includes all files relevant to the paper "NewsUnfold: Creating a News-Reading Application That Indicates Linguistic
Media Bias and Collects Feedback."

# Abstract

Media bias is a multifaceted problem, leading to one-sided views and impacting decision-making. A way to address bias in news articles is to automatically detect and indicate it through machine-learning methods. However, such detection is limited due to the difficulty of obtaining reliable training data. To facilitate the data-gathering process, we introduce NewsUnfold, a news-reading web application leveraging an initially tested feedback mechanism to collect reader feedback on machine-generated bias highlights within news articles. Our approach augments dataset quality by significantly increasing inter-annotator agreement by 26.31% and improving classifier performance by 2.49%. As the first human-in-the-loop application for media bias, NewsUnfold shows that a user-centric approach to media bias data collection can return reliable data while being scalable and evaluated as easy to use. NewsUnfold demonstrates that feedback mechanisms are a promising strategy to reduce data collection expenses, fluidly adapt to changes in language, and enhance evaluators' diversity.

## Content
- [News Ninja Source Code](/NewsUnfold%20Code)

- [News Ninja Dataset](/NewsUnfold%20Data)

- [Video of News Ninja](https://youtu.be/h4hd9p8MECo)

## About the NUDA Dataset
Media bias is a multifaceted problem, leading to one-sided views and impacting decision-making. A way to address bias in news articles is to automatically detect and indicate it through machine-learning methods. However, such detection is limited due to the difficulty of obtaining reliable training data. To facilitate the data-gathering process, we introduce NewsUnfold, a news-reading web application leveraging an initially tested feedback mechanism to collect reader feedback on machine-generated bias highlights within news articles. Our approach augments dataset quality by significantly increasing inter-annotator agreement by 26.31% and improving classifier performance by 2.49%. As the first human-in-the-loop application for media bias, NewsUnfold shows that a user-centric approach to media bias data collection can return reliable data while being scalable and evaluated as easy to use. NewsUnfold demonstrates that feedback mechanisms are a promising strategy to reduce data collection expenses, fluidly adapt to changes in language, and enhance evaluators' diversity.

### General

This dataset was created through user feedback on automatically generated bias highlights on news articles on the website NewsUnfold made by ANON. Its goal is to improve the detection of linguistic media bias for analysis and to indicate it to the public. Support came from ANON. None of the funders played any role in the dataset creation process or publication-related decisions.

The dataset consists of text, namely biased sentences with binary bias labels (processed, biased or not biased) as well as metadata about the article. It includes all feedback that was given. The single ratings (unprocessed) used to create the labels with correlating User IDs are included.

For training, this dataset was combined with the BABE dataset.  All data is completely anonymous. Some sentences might be offensive or triggering as they were taken from biased or more extreme news sources. The dataset does not identify sub-populations or can be considered sensitive to them, nor is it possible to identify individuals.

### Description of the Data Files

This repository contains the datasets for the anonymous NewsUnfold submission. The tables contain the following data:

NUDAdataset.csv: the NUDA dataset with 310 new sentences with bias labels
Statistics.png: contains all Umami statistics for NewsUnfold's usage data
Feedback.csv: holds the participantID of a single feedback with the sentence ID (contentId), the bias rating, and provided reasons
Content.csv: holds the participant ID of a rating with the sentence ID (contentId) of a rated sentence and the bias rating, and reason, if given
Article.csv: holds the article ID, title, source, article metadata, article topic, and bias amount in %
Participant.csv: holds the participant IDs and data processing consent

### Collection Process

Data was collected through interactions with the Feedback Mechanism on NewsUnfold. A news article was displayed with automatically generated bias highlights. Each highlight could be selected, and readers were able to agree or disagree with the automatic label. Through a majority vote, labels were generated from those feedback interactions. Spammers were excluded through a spam detection approach.

Readers came to our website voluntarily through posts on LinkedIn and social media as well as posts on university boards. The data collection period lasted for one week, from March 4th to March 11th (2023). The landing page informed them about the goal and the data processing. After being informed, they could proceed to the article overview.

So far, the dataset has been used on top of BABE to train a linguistic bias classifier, adopting hyperparameter configurations from BABE with a pre-trained model from Hugging Face.
The dataset will be open source. On acceptance, a link with all details and contact information will be provided. No third parties are involved.

The dataset will not be maintained as it captures the first test of NewsUnfold at a specific point in time. However, new datasets will arise from further iterations. Those will be linked in the repository. Please cite the NewsUnfold paper if you use the dataset and contact us if you're interested in more information or joining the project.

# Cite 

Hinterreiter, S., Wessel, M., Schliski, F., Echizen, I., Latoschik, M.E., and Spinde, T. (2025). NewsUnfold: Creating a News-Reading Application That Indicates Linguistic
Media Bias and Collects Feedback. Conditionally accepted at Proceedings of the International AAAI Conference on Web and Social Media, 19. 
