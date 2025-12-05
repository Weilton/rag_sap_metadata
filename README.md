# rag_sap_metadata
Mini RAG project for SAP metadata (DDL / ERD) focused on QMEL, MARA, KNA1 tables

Flow:
1. Defines fake metadata for tables and relationships.
2. Generates descriptive text blocks (per table, per relationship).
3. Creates simple bag-of-word embeddings.
4. Implements similarity search (cosine).
5. Implements answer_question simulating RAG.

To adapt to a real environment:
- Replace METADATA_FAKE with reading metadata tables (SAP, Databricks, Glue, etc.).
- Replace llm_fake(prompt) with a real call to OpenAI / Bedrock / another LLM.
