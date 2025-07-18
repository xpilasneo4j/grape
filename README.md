# GRAPE

**Graph Retriever Analysis and Performance Evaluation**

**GRAPE** is a framework for benchmarking how well LLM agents query knowledge graphs via MCP-compatible servers.

### Structure

* `evaluation-dataset-generation/` – Uses LLMs to generate questions and answers from real Neo4j databases
* `mcp-server-evaluations/` – Evaluates MCP server implementations against the generated dataset using an LLM judge

GRAPE supports multiple domains, real-world graphs from [demo.neo4jlabs.com](https://demo.neo4jlabs.com), and a consistent evaluation pipeline.

### How to Start

1. **Use the existing dataset**
   The repository includes a pre-generated `generated_dataset.json`.
   Re-running `dataset_generation.ipynb` is optional.

2. **Run evaluation**
   Go to a folder in `mcp-server-evaluations/` and run the evaluation notebook with the dataset.

### Contribute

* Add various MCP implementation evaluations
