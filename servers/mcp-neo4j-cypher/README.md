# mcp-neo4j-cypher

This project evaluates **`mcp-neo4j-cypher`** in the accompanying evaluation notebook.

The `mcp-neo4j-cypher` server allows an LLM agent to extract the Neo4j database schema and generate Cypher queries to read from and update the graph.

### Available Tools

* **`get-neo4j-schema`** – Extracts the graph schema.
* **`read-neo4j-cypher`** – Executes read-only Cypher queries.
* **`write-neo4j-cypher`** – Executes Cypher write/update operations.

**Repo:** [neo4j-contrib/mcp-neo4j-cypher](https://github.com/neo4j-contrib/mcp-neo4j/tree/main/servers/mcp-neo4j-cypher)
**Docs:** [Neo4j Developer Guide](https://neo4j.com/developer/genai-ecosystem/model-context-protocol-mcp/#_mcp_neo4j_cypher)