## Facebook Live Sellers in Thailand

In this project, the **CRISP-DM (Cross-Industry Standard Process for Data Mining)** methodology has been used.


https://www.sv-europe.com/crisp-dm-methodology/


### 1.Business Understanding

Goal: Analyze user engagement patterns (comments, reactions, shares) in response to content posted by fashion and cosmetics sellers on Facebook to identify effective sales and engagement strategies.



### 2.Data Understanding

Understand data collection process :
ta Source: Facebook posts from 10 Live sellers in fashion and cosmetics (7050 instances, 11 features).

Main Features (Variables) of the Data:

status_type: Type of post (video, photo, link, text status)

num_comments: Number of user comments under each post

num_shares: Number of times the post was shared by users

num_reactions: Total number of user reactions (such as like, love, wow, etc.)

num_likes / num_loves / num_wows / num_hahas / num_sads / num_angrys: Breakdown of each specific Facebook reaction

status_published: Date and time the post was published

video_id / status_id / message: Internal identifiers related to each post (usually dropped or summarized during analysis)



### 3.Data Preparation


### 4.Modeling


### 5.Evaluation

In the evaluation phase of this project, we assessed the quality of the clustering results using the Silhouette Score metric. This metric quantifies how well each data point fits within its assigned cluster compared to other clusters. A higher Silhouette Score indicates better-defined clusters.

We applied and compared the following clustering algorithms:

KMeans: Silhouette Score = 0.37

Gaussian Mixture Model (GMM): Silhouette Score = 0.23

Agglomerative Clustering: Silhouette Score = 0.54

DBSCAN: Silhouette Score = 0.22

Among all models, Agglomerative Clustering achieved the highest Silhouette Score of 0.54, suggesting that it produced the most cohesive and well-separated clusters.

In addition to the quantitative evaluation, we also conducted a qualitative analysis by examining the mean values of key features within each cluster. The clusters revealed distinct behavioral patterns in terms of reactions, comments, and shares, confirming that the clustering results are meaningful and interpretable.

Based on both quantitative and qualitative assessments, Agglomerative Clustering was selected as the best-performing model for this project.

