# Analyzing Social Networks using GraphX/GraphFrame

This project demonstrates the use of Spark's GraphX/GraphFrame to analyze social network data. The project allows users to choose any dataset available from the SNAP repository to perform various operations and algorithms on a graph representation of the social network data.

## Table of Contents
- [Introduction](#introduction)
- [Requirements](#requirements)
- [Usage](#usage)
  - [Loading Data](#loading-data)
  - [Create Graphs](#create-graphs)
  - [Running Queries](#running-queries)
    - [a. Outdegree Analysis](#outdegree-analysis)
    - [b. Indegree Analysis](#indegree-analysis)
    - [c. PageRank Calculation](#pagerank-calculation)
    - [d. Connected Components](#connected-components)
    - [e. Triangle Counts](#triangle-counts)
- [Notebook Usage](#notebook-usage)

## Introduction

The purpose of this project is to utilize Spark's GraphX/GraphFrame library to perform analysis and execute various algorithms on social network datasets available from the SNAP repository. Users can execute tasks such as finding top nodes based on outdegree, indegree, calculating PageRank, identifying connected components, and obtaining triangle counts.

## Requirements

To run this project, you'll need:
- Apache Spark
- GraphX/GraphFrame library
- Social network dataset from the SNAP repository

## Usage

### Loading Data

1. Load the social network dataset into a GraphFrame or RDD using Spark.
2. Define a parser to extract relevant fields from the dataset.
3. Note: Convert undirected relationships into directed relationships if necessary.

### Create Graphs

1. Define the edge and vertex structure.
2. Create property graphs based on the dataset.

### Running Queries

#### a. Outdegree Analysis

Find the top 5 nodes with the highest outdegree and count the number of outgoing edges for each.

#### b. Indegree Analysis

Find the top 5 nodes with the highest indegree and count the number of incoming edges for each.

#### c. PageRank Calculation

Calculate PageRank for each node and output the top 5 nodes with the highest PageRank values.

#### d. Connected Components

Run the connected components algorithm and find the top 5 components with the largest number of nodes.

#### e. Triangle Counts

Run the triangle counts algorithm on each vertex and output the top 5 vertices with the largest triangle count. In case of ties, randomly select the top 5 vertices.

## Notebook Usage

Refer to the provided notebook in this repository for a step-by-step guide and code implementation of the mentioned tasks.
