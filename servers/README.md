# MCP servers evaluation

This folder contains multiple server setups for evaluating how well LLM agents query knowledge graphs via tool-based interfaces.

Each subdirectory:

* Implements or reuses an MCP-compatible server
* Evaluates it against a shared dataset using the provided notebook or script

### Evaluation

We use an LLM as a judge to assess the quality of responses across different categories of questions.

### Structure

```
/
├── mcp-neo4j-cypher/     # Uses existing mcp-neo4j-cypher server
├── my-custom-server/     # Custom MCP-compatible server
...
```

Evaluations focus on how effectively each server enables agent-based querying of knowledge graphs.