# databricks_genAI_demo

Companion code for a Medium series on building production-grade GenAI agents with LangGraph on Databricks Free Edition. Notebooks here are designed to be forked, opened in your own Free Edition workspace, and run top to bottom.

This is a learning repo, not a production-ready system. Code is kept deliberately small so the moving parts are easy to read.

## The series

1. [What clearing the Databricks GenAI exam taught me about my own LangGraph project](https://medium.com/@kapadiadarshil25/what-clearing-the-databricks-genai-exam-taught-me-about-my-own-langgraph-project-4ca9147b9c44) — the reflection post that kicked this off
2. **Setting up Databricks Free Edition** *(link will be added once published)* — companion to `notebooks/01_first_table.ipynb`
3. Coming soon: Unity Catalog row filters for a multi-tenant agent
4. Coming soon: A small LangGraph agent on top of Databricks Foundation Model API
5. Coming soon: MLflow 3.0 tracing for multi-node agents
6. Coming soon: Mosaic AI Agent Evaluation in practice

## What you need to run this

- A Databricks Free Edition account ([sign up here](https://www.databricks.com/learn/free-edition)) — free, no credit card, perpetual
- Serverless compute, which Free Edition gives you by default
- Basic familiarity with Python and SQL

## Repo structure

```
databricks_genAI_demo/
├── README.md
├── LICENSE
└── notebooks/
    └── 01_first_table.ipynb   # First post — catalog, schema, and a fake customers table
```

More notebooks will be added as the series progresses.

## How to use a notebook

1. Open your Databricks Free Edition workspace.
2. In the left sidebar, go to **Workspace** → click the **Import** button (or right-click any folder → Import).
3. Upload the `.ipynb` file from this repo.
4. Open the imported notebook and attach it to **Serverless** compute (top-right dropdown).
5. Run cells top to bottom.

Each notebook assumes the catalog and schema referenced in it already exist. Notebook `01_first_table.ipynb` assumes a catalog called `nocompany` and a schema called `demo`. Create these once via Catalog Explorer (Catalog → Create → Catalog / Schema) before running.

## A note on the data

All data used in this repo is synthetic and generated using [Faker](https://faker.readthedocs.io/). The fictional company "NoCompany" exists only here. No real client data, no proprietary schemas, nothing scraped from anywhere. The whole point is that you can fork this, run it, and not worry about where the data came from.

## Reporting issues

If something here breaks or feels unclear, open an issue on the repo or leave a response on the corresponding Medium post. The series is a work in progress and feedback shapes future notebooks.

## License

MIT. Use it, fork it, copy it, modify it. Attribution appreciated but not required.