# Ted4j

## What is Ted4j project?
**Ted4j** is a [Neo4j](https://neo4j.com/) GraphDB based collection of all past [TED](https://www.ted.com/) speeches.

## Why?
Mainly for 2 reasons:
1. Let you analyze relationships in TED world, such as shortest paths between authors, common talk themes and so on... A sort of little PoC of GraphDB potentials
2. Play with Neo4j and Python, during a boring evening

## How I made this?
Ted4j is based on:
1. [TED](https://www.ted.com/) (obviously), as data source
2. [Neo4j](https://neo4j.com/), for data storage and analysis purposes
3. [Python 3.6](https://www.python.org/) with , for data extraction from TED and load to Neo4j.
⋅⋅⋅3.1. [Scrapy](https://scrapy.org/) library, for information extraction and web scraping
⋅⋅⋅3.2. [Neo4j Python Driver](https://neo4j.com/developer/python/#neo4j-python-driver) library, for Neo4j interface and load

Right now, I'll not load Python script to GitHub: it's really rough and doesn't bring any added value.

# Quick Start
You can install Ted4j DB in 5 steps as follows.

## Step1: Download Neo4j
First, download [Neo4j graph-database](https://neo4j.com/download/). Notice that Ted4j has been tested on Neo4j 3.3.4. I suggest you to download Neo4j Desktop and then to deploy a new GraphDB instance using the Neo4j 3.3.4.
## Step2: Download GraphDBLP database dump 
Download the [dump file](../database/Ted4j.dump)
