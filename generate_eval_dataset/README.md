# evaluation-dataset-generation

This folder contains code and prompts for generating the evaluation dataset used to benchmark MCP server implementations.

We use LLMs to generate:

* Natural language questions across multiple categories
* Ground truth answers (in Cypher or plain text, depending on the task)

### Data Sources

The dataset is based on **five Neo4j databases** hosted at [demo.neo4jlabs.com](https://demo.neo4jlabs.com), each representing a different domain for evaluation.

### Code Structure

* `dataset_generation.ipynb` – Main notebook for generating the dataset
* `prompts.py` – Prompt templates for question and answer generation
* `utils.py` – Helper functions for database access and formatting
* `generated_dataset.json` – Final output containing questions, answers, and metadata

The generated dataset is used to evaluate how well MCP-compatible servers support agent-based querying over real-world knowledge graphs.
