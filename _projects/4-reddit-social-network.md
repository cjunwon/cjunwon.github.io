---
title: "Developing efficient classification for Reddit posts/comments/communities with Graph Neural Networks (GNNs)"
excerpt: "DataRes Research (UCLA), Winter 2023<br/><br/><img src='/images/datares_research_winer_2023_slide_1.png' style='box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.3);'>"
collection: projects
---

### Background

Reddit is a social media platform where users can post, comment, and upvote/downvote on various topics. Reddit is divided into subcommunities (subreddits) based on topics of interest. This platform is a rich source of data for studying social networks and community detection.

A person's affiliation with communities can be predicted based on various features, such as their demographic, language use, clickstream, etc. While we can use these features to predict a person's affiliation with a community through traditional classification models, we can also use the graph structure of the entire platform to predict a person's affiliation with a community. 

This project aims to efficiently discover subcommunities and their changes using the pure graph structure of the entire Reddit platform, constructed solely from the interactions between users and posts (likes, comments, etc.) and avoiding the use of other categorical features. This project also performs node classification on new posts/comments.

### Objective

* Collect community data and set up environment
  * Pull in community data using PyTorch Geometric (Reddit dataset)
  * Connect to remote workstation through SSH (sponsored by AI Safety at UCLA)
* Test and validate various community detection models
  * GraphSAGE
  * Graph Attention Networks
  * FlashAttention

<!-- ### Tools & Technologies

<table style="width:100%">
  <tr>
    <th>Target</th>
    <th>Task</th> 
    <th>Tools/Packages Used</th>
  </tr>
  <tr>
    <td>Data Collection</td>
    <td>Pull in Reddit dataset from PyTorch Geometric pacakage, including nodes, edges, features, classes</td> 
    <td>PyTorch Geometric</td>
  </tr>
  <tr>
    <td>Data Pre-processing</td>
    <td>Subset dataset for handling and testing</td> 
    <td>numpy</td>
  </tr>
  <tr>
    <td>Model Implementation</td>
    <td>...</td> 
    <td>PyTorch, GraphSAGE, Graph Attention Networks, FlashAttention</td>
  </tr>
  <tr>
    <td>Model Evaluation</td>
    <td>Compare model performances for community detection</td> 
    <td>PyTorch, scikit-learn, Matplotlib</td>
  </tr>
</table><br> -->

### Relevant Files

* Code for this project is available on [GitHub](https://github.com/cjunwon/Reddit-Social-Network-Analysis/tree/master).

The following slides were presented during the quarterly DataRes Demo Day at UCLA.

[Download  PDF](/files/datares_research_winter_2023.pdf)

<iframe src="/files/datares_research_winter_2023.pdf" width="100%" height="500"></iframe>