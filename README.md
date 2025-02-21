# Chronographic EU Voting Patterns
You can optimize petition timings within the EU. That's a problem haha. This repo plays with VoteWatchers European Parliament dataset to find contributing variables in voting patterns. 

## Trend Examples:

Pairwise Similaities between voters, first 46 MEPs alphabetically:

![image](https://github.com/user-attachments/assets/aa730087-bdaf-4692-af91-e2895bdd8f87)

2D Voting patterns colourd by European Parliament Group:

![image](https://github.com/user-attachments/assets/fb7c66f1-894f-484a-8ae5-4dcc7845e111)

3D graph example (interactive during runtime):

![image](https://github.com/user-attachments/assets/db73a0ef-7214-4618-9828-ae042dd9005c)


## Mathematics
#### Similarity Measure
I invented a simple probabilistic measure:

![image](https://github.com/user-attachments/assets/aedf8abf-6b6d-4a5c-ac7c-ccd0c86a7e27)

#### Multidimensional Scaling [MDS]
I used the classical MDS. I learnt that voting similarities are non-euclidean A clear improvement is to use a non-euclidean MDS.

## How to Run
The python files are really easy to read. But for ease:
1. Download Votewatch Europe dataset
2. Run epg_and_nation_clustering to see patterns of ALL votes over the interval you select. The file plots in 2D, 3D, and does a 7D radial projection.
3. Run voting_patterns_over_years to select categories of petitions to see how they change year by year or quarter by quarter.

## Analysis
See report.pdf for a subset of the analysis of results this repo produces.

## VoteWatch Europe dataset
Part of its description: "VoteWatch Europe provides roll-call data and voting information for the European Parliament and the EU Council from 2004 to 2022. The VoteWatch project was founded by Simon Hix, Doru Frantescu and Sara Hagemann, and uses roll-call data collection and analysis techniques developed by Prof. Hix and Prof. Abdul Noury." 

It is a **fantastic** Creative Commons Attribution 4.0 International good. 

## Dependencies
1. The dataset for the relevant years in the same folder: https://cadmus.eui.eu/handle/1814/74918
2. Modules listed in requirements.txt


   
