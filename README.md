# WikiPathwaysInteractions
Jupyter Notebook SPARQL queries against the WikiPathways SPARQL Endpoint
# Supplementary information 

This repository has Jupyter Notebook queries that supplement this paper:

```text
Understanding signaling and metabolic paths using semantified and harmonized information about biological interactions
Ryan A Miller, Martina Kutmon, Anwesha Bohler, Andra Waagmeester, Chris T Evelo, Egon L Willighagen
doi: https://doi.org/10.1371/JOURNAL.PONE.0263057
```

Queries are represented in Jupyter Notebooks using Python against the WikiPathways SPARQL endpoint (http://sparql.wikipathways.org/).

## Python Jupyter Notebooks

These are the queries that are used to query the WikiPathways SPARQL endpoint.  Results of the queries are displayed in tabular format.  For each query, users can also locate the SPARQL query in the Python code and copy the query section making sure to only copy text between the quotation marks "".  The query can be identified in the Python code by locating the "PathwayQuery" variable.  The user can then paste the copied query into the SPARQL endpoint (http://sparql.wikipathways.org/) if they wish to edit the query to their liking and then select the "Run Query" button on the Virtuoso page to perform their own custom version of the copied query.  

## Included types of Interactions

Interactions are represented for general WikiPathways interaction types, but also includes MIM and SBGN notations for added options for drawing pathways in the user's preferred type.  
