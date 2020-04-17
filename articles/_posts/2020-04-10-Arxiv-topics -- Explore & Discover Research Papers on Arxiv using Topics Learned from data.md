# Arxiv-topics: Explore & Discover Research Papers on Arxiv repository using Topics Learned from data
##

[Arxiv repository](https://arxiv.org) hosts 1.5m academic papers, and users add over 10K papers per month. Keeping track of trends is challenging as it is limited to keyword search, and does not let users track and explore content based on themes that capture relationships beyond shared words, or recommend content from this perspective. This challenged us to use unsupervised learning to learn topics to summarise documents, and let users explore and find research papers on similar topics.

Our approach is divided in three steps:

First, For the topic discovery we used LDA topic model. In simple terms, with given documents and their words, the purpose of LDA is to learn the representation of fixed number of topics from the corpus and their distribution. We also experimented with  with other topic models such as LSA, contrasted their result and found LDA topics to be more accurate and interpretable.

Second, At the core of our web application, we use pyLDAvis, to visualize and let user explore individual topics and its associated terms.
Whats new in our approach is third step which now allow user to find research paper similar to its topic mix. For example, a user reading research paper on theme of Computer vision and Human Computer Interaction. can easily find another paper around same theme.

For experiments we  download 26,000 research papers through [Arxiv api: https://arxiv.org/help/api/index](https://arxiv.org/help/api/index), lemmatised them, applied stemming, and examined top 1000 keywords manually

To evaluate a topic model, we calculated Topic coherence which is measures of topic consistency. Since it is unsupervised learning for our experiments we generated visualisations of over a topic range from 3 to 100. Experiment resulted in topics which are diverse yet well defined and can be given well defined names like Language, LifeScience, Theory etc.

## Quick walkthrough video with demo
###### (3 min watch)
-----
[![You tube video](https://raw.githubusercontent.com/fakemonk1/arxiv-topics/master/documents/Screenshot2.png)](https://www.youtube.com/watch?v=7uf5MMTe2CU "Quick walkthrough video with demo  - Click to Watch!")

## Running app demo (on Heroku)
###### (Please allow 30 sec to initialize the instance
-----
[![Demo screenshot](https://raw.githubusercontent.com/fakemonk1/arxiv-topics/master/documents/screenshot-demo.png)](https://boiling-thicket-31500.herokuapp.com/ "Demo on Heroku  - Click to view!")

## Detailed project details
###### 15 min read
-----
[Detailed  Report PDF ](https://github.com/fakemonk1/arxiv-topics/blob/master/documents/report.pdf)