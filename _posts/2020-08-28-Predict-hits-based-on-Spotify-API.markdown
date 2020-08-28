---
layout: post
title: Predict hits based on Spotify API
date: 2020-08-28 12:00:00 +0200
description: Machine Learning applied to Spotify audio features for a classification task. # Add post description (optional)
img: spot-it.png # Add image post (optional)
tags: [classification, music, ml, anomaly, imbalanced, dataset] # add tag
---
**Machine Learning applied to Spotify audio features for a classification task.**

## Context and problem
I am a big user of Spotify and a musician, so this first project was kind of obvious. The idea is to use Spotify's API to retrieve data about songs (mainly audio features) and see if we can predict if a song will be a hit or not based on these features.

To be more precise about the process that we will follow here:
- I will retrieve hit songs based on Billboard charts.
- Then I will use Spotify API to get random songs that are not hits and try to have a 10/90 ratio between hits and non-hits to "respect" a natural imbalanced distribution (in fact it should be even more imbalanced!)
- I will call the Spotify API another time to get the audio features and build the dataset.
- Finally, I will perform EDA and multiple Machine Learning approach to classify a song (hit or not), so it will be a classical binary classification problem.

Let's start!

## Creation of the dataset
First, we have to build our raw material: the dataset! It is an important part as we want our data to be quite representative of all (or almost) possible songs.
The very first step is to find a list of hit songs, preferably over several years. Luckily, I found on [Dataworld](https://data.world/kcmillersean/billboard-hot-100-1958-2017/workspace/file?filename=Hot+Stuff.csv) this csv file contains all songs that have been at least 1 week in the Top 100 Billboard chart from 1958 to 2018.

//To be continued//

```python
# Data manipulation
import numpy as np
import pandas as pd
```
