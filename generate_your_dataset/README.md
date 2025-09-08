# evaluation-dataset-generation

This folder contains code and prompts for generating the evaluation dataset used to benchmark MCP server implementations.

We use LLMs to generate:

* Natural language questions across multiple categories
* Ground truth answers (in Cypher or plain text, depending on the task)

### Code Structure

* `dataset_generation.ipynb` – Main notebook for generating the dataset
* `prompts.py` – Prompt templates for question and answer generation
* `utils.py` – Helper functions for database access and formatting
* `generated_dataset_<timestamp>.json` – Final output containing questions, answers, and metadata
* `template.env` - example on how to provide the parameters
* 
### env file Structure

* LLM_CREATES, list of models to be used. Defined as a list of tring pairs ["LLM Type", "Model Name", "API key"]
* LLM_QA, LLM used for validating. Can be GOOGLE or CLAUDE
* LLM_QA_MODEL, Model used for validating. Has to be a model available on the LLM provided in LLM_QA
* LLM_QA_API_KEY, api key used for this LLM
* DATABASES, list of databases used for the Q&A generation. Defined as a list of String quadruplet ["db name", "login", "pwd", "uri"]

The generated dataset is used to evaluate how well MCP-compatible servers support agent-based querying over real-world knowledge graphs.
