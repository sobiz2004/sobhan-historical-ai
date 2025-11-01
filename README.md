# Historical AI Agent
## Overview

This project was developed as part of the Advanced Programming course under the supervision of Dr. Hossein Khani at Sharif University of Technology.
The goal of this project was to design an AI Agent capable of answering questions about historical figures from different eras and regions using a knowledge graph and LLM-based query processing.

## Project Description

The system integrates Neo4j, a graph database, with an LLM-powered reasoning engine to process natural-language questions about historical individuals and their relations.

1. Dataset Construction

A custom dataset of famous historical figures across various periods and civilizations was created. Each person’s information (e.g., name, era, country, relations, achievements) was stored as nodes and edges in a Neo4j graph.

2. Graph Database (Neo4j)

Neo4j was used to represent relationships.

3. AI Agent (Java)

The core agent was implemented in Java, managing user input, graph queries, and output generation.
It connects to the Neo4j database via its official driver to execute Cypher queries dynamically.

4. LLM Integration (Ollama)

The system uses Ollama, a lightweight local LLM interface, to interpret natural-language queries and translate them into meaningful Cypher queries for Neo4j.
The agent then formats and presents the retrieved information in human-readable form.


## Technologies Used

Java 17

Neo4j Graph Database

Ollama LLM Framework

Cypher Query Language

Maven (for dependency management)

## How to Run

Install and start Neo4j locally.

Import the dataset (historical_people.csv or similar).

Configure the database credentials in config.properties.

Run the Java project:

mvn clean compile exec:java


Make sure Ollama is running locally and connected via API.

## Future Work

Improve the natural language understanding of complex multi-hop questions.

Extend the dataset with temporal and geographical metadata.

Integrate visualization for graph query results.

## Author

Sobhan Zamani Kiasari, B.Sc. Computer Engineering, Sharif University of Technology

sobhanzkia04@gmail.com
