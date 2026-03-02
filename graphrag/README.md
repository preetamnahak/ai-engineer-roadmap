The notebook is just to give you a gist of what a graphrag actually is.


Real GraphRAG Pipeline (Production View)

In a real system, you would:

1️⃣ Chunk document
2️⃣ Use LLM to extract triples and resolve conflcits with existing similar entites in your graphdb
3️⃣ Store in dGraph/TigerGraph/Neo4j graph dbs
4️⃣ On query:
    Detect entities
    Expand neighbors (1-hop, 2-hop)
    Rank subgraph
    Send structured context to LLM