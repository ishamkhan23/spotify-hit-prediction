Predicting Hit Songs on Spotify

This repository contains the code and report for our CS 439 Data Science course project, where we explore unsupervised learning techniques to uncover latent musical structures and seasonal trends in Spotify streaming data.

Project Overview

Streaming platforms release tens of thousands of new tracks daily, yet promotional resources are limited. We ask whether open, transparent methods can:

Discover genre/mood clusters without using any human-provided labels.

Reveal seasonal listening patterns, like “summer anthems” and “winter chill.”

Characterize audio and engagement features—energy, danceability, acousticness, playlist presence—that define hit-worthy music.

Our pipeline uses:

Data preprocessing: cleaning, log-transforming heavy-tailed features, merging correlated playlist counts.

Dimensionality reduction: PCA to condense 44 features into three principal components.

Hierarchical clustering: Ward linkage to identify three natural song groups (hype, mainstream, R&B).

Seasonality analysis: Heat-maps and PCA scatters to track cluster prevalence over months.

Repository Contents

FinalNotebook.ipynb: Jupyter notebook executing the full analysis end-to-end.


Getting Started

Clone the repo

git clone https://github.com/ishamkhan23/spotify-hit-prediction.git
cd spotify-hit-prediction

Install dependencies

pip install -r requirements.txt

Run the notebook

jupyter lab PredictHitSongs.ipynb

View the report
Open FinalReport.md in Markdown preview or your favorite text editor.

Key Findings

Clusters: Three distinct song clusters emerged—high-energy hype tracks, mainstream pop, and R&B-style love songs.

Seasonality: Hype tracks peak in summer; R&B love songs dominate winter; mainstream pop remains steady year-round.

Features: Energy and danceability drove cluster separation, while playlist presence was uniformly distributed, showing curator consistency.

Future Work

Extend analysis across multiple years to track micro-genre evolution.

Incorporate regional charts to test global applicability.

Develop interactive dashboards for A&R teams to explore clusters and seasonality in real time.


