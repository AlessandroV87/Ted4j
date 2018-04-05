# Ted4j

## What is Ted4j project?
**Ted4j** is a [Neo4j](https://neo4j.com/) GraphDB based collection of all past [TED](https://www.ted.com/) speeches.

## Why?
Mainly for 2 reasons:
1. Let you analyse relationships in TED world, such as shortest paths between authors, common talk themes and so on... A sort of little PoC of GraphDB potentials
2. Play with Neo4j and Python, during a boring evening

## How it's made?
Ted4j is based on:
1. [TED](https://www.ted.com/) (obviously), as data source
2. [Neo4j](https://neo4j.com/), for data storage and analysis purposes
3. [Python 3.6](https://www.python.org/), for data extraction from TED and load to Neo4j.
   - [Scrapy](https://scrapy.org/) library, for information extraction and web scraping
   - [Neo4j Python Driver](https://neo4j.com/developer/python/#neo4j-python-driver) library, for Neo4j interface and load

Right now, I'll not load Python script to GitHub: it's really rough and doesn't bring any added value.

# Quick Start
You can install Ted4j DB in 5 steps as follows.

## Step1: Download Neo4j
First, download and install [Neo4j Desktop](https://neo4j.com/download/). Notice that Ted4j has been tested on Neo4j 3.3.4. I suggest you to download Neo4j Desktop and then to deploy a new GraphDB instance using the Neo4j 3.3.4.
## Step2: Download Ted4j database dump 
Download the [dump file](./database/Ted4j.dump) that contains the whole GraphDB in a local folder (e.g., Download).
## Step3: Create an empty Neo4j database
Open Neo4j Desktop previously installed. On the main screen, create a new project (eg: "Ted4j"). Inside your new project, click on "Create a Local Graph" and set a preferred name and a password. Keep in mind to select version 3.3.4, to make sure it will be compatible with Ted4j dump file. **Don't start your DB, for now: we need it to be stopped to allow you to restore the dump file**
## Step4: Restore Ted4j dump
On your GraphDB project page, press "Manage" and then "Terminal". Here, write: `bin/neo4j-admin load --from=<path_to_your_donwload_folder>/Ted4j.dump --force`. This command will restore Ted4j on your DB. This operation may take a while. Please do not close the window while running.
## Step5: Run Ted4j
Just press the Start button to run your Ted4j instance. Then click on "Open Browser" to access Neo4j Desktop Browser and navigate. In a short time I'll post a couple of query examples.
