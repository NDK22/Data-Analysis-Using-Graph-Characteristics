# DBLP Data Analysis Using Graph Characteristics
## Project II - Team 18 - Fall 2022

### Report By:
Nikhil Das Karavatt
Student ID: 1002085391

## Table of Contents
1. [Overview](#overview)
2. [File Descriptions](#file-descriptions)
3. [Division of Labour](#division-of-labour)
4. [Problems Encountered](#problems-encountered)
5. [Analysis](#analysis)
   - [Analysis 0](#analysis-0)
   - [Analysis 1](#analysis-1)
   - [Analysis 2](#analysis-2)
   - [Analysis 3.2](#analysis-32)

## Overview
This report documents the analysis of a large DBLP dataset, focusing on various aspects such as authors, references, venues, and more. The project explores the domains, applications, and challenges related to Python and its libraries, particularly in the field of graph analysis and visualization.

The project involved uploading the DBLP dataset to Google Drive, reading the data in Google Colab in chunks, preprocessing the data, and performing graph analysis. Three main graphs were created:

1. **Known Author Graph**: An undirected graph connecting authors related to each other.
2. **Paper Citation Graph**: A directed graph connecting paper IDs with their references.
3. **Author Venue Graph**: An undirected graph connecting authors to the venues where they presented their papers.

## File Descriptions
The project includes various files, primarily in .csv and .txt formats:

- `dblp_v10.zip`: Input file containing the DBLP dataset in JSON format.
- `author_edge_list_5.txt`: Edge list of the Known Author Graph (sample size 5).
- `author_edge_list_output_5.txt`: Output of Known Author Graph characteristics (sample size 5).
- `author_edge_list_20.txt`: Edge list of the Known Author Graph (sample size 20,000).
- `author_edge_list_output_20.txt`: Output of Known Author Graph characteristics (sample size 20,000).
- `reference_id_edge_list_5.txt`: Edge list of the Paper Citation Graph (sample size 5).
- `reference_id_edge_list_output_5.txt`: Output of Paper Citation Graph characteristics (sample size 5).
- `reference_id_edge_list_20.txt`: Edge list of the Paper Citation Graph (sample size 20,000).
- `reference_id_edge_list_output_20.txt`: Output of Paper Citation Graph characteristics (sample size 20,000).
- `author_venue_edge_list_5.txt`: Edge list of the Author Venue Graph (sample size 5).
- `author_venue_edge_list_output_5.txt`: Output of Author Venue Graph characteristics (sample size 5).
- `author_venue_edge_list_20.txt`: Edge list of the Author Venue Graph (sample size 20,000).
- `author_venue_edge_list_output_20.txt`: Output of Author Venue Graph characteristics (sample size 20,000).
- `DASC5300_Proj2_Fall22_team_18.ipynb`: Jupyter Notebook containing the code for data analysis.

## Division of Labour
The project was completed individually, taking approximately 60 hours of work to finish.

## Problems Encountered
1. Self-node Issue: While creating edges for the Known Author Graph, a self-node issue (A1, A1) was encountered, which was fixed by refining the edge creation code and using a predefined function to remove self-loops.
2. Graph Layout: Graph layout overlapping was resolved by adjusting parameters to improve graph readability.
3. Data Cleaning: Cleaning data with NaN values and empty sets required careful handling to avoid unnecessary row drops.

## Analysis
### Analysis 0
A sample size of 20,000 was used to calculate graph characteristics for Known Author Graph, Paper Citation Graph, and Author Venue Graph:

**Known Author Graph:**
- Number of Nodes: 50,436
- Number of Edges: 90,153
- Density: 7.0882e-05
- Number of Connected Components: 11,064
- Diameter: -1
- Minimum Degree: 1
- Maximum Degree: 53
- Average Degree: 3.5749
- Std Dev of Degree: 3.3221

**Paper Citation Graph:**
- Number of Nodes: 133,329
- Number of Edges: 155,457
- Density: 1.7490e-05
- Number of Connected Components: 3,613
- Diameter: -1
- Minimum Degree: 1
- Maximum Degree: 153
- Average Degree: 2.3319
- Std Dev of Degree: 4.3629

**Author Venue Graph:**
- Number of Nodes: 8,805
- Number of Edges: 6,646
- Density: 0.0001715
- Number of Connected Components: 2,168
- Diameter: -1
- Minimum Degree: 1
- Maximum Degree: 19
- Average Degree: 1.5096
- Std Dev of Degree: 1.1879

### Analysis 1
Comparison between manually calculated and coded graph characteristics for Known Author Graph, Paper Citation Graph, and Author Venue Graph.

### Analysis 2
Identification of the most common clique size in the Known Author Graph.

### Analysis 3.2
Identification of the top 10 most cited papers in the Paper Citation Graph.

## Ground Truth
The report includes ground truth information for Known Author Graph and manual calculations for several graph characteristics.
