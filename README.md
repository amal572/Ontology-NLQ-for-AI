# Ontology NLQ for AI - Data Mining Project

This project focuses on developing an algorithm to standardize different ontologies according to the structure provided by the subject teacher. The ontologies consist of multiple XML files, each containing the name of an AI algorithm and its relation to it. The primary objective is to enable efficient searching within these ontologies using natural language queries, which are then converted into SPARQL language for querying.

## Approach

1. **Standardization of Ontologies:** We start by iterating through all ontology class names and apply fuzzy set matching to determine if the names match or not. If discrepancies are found, we replace them with the corresponding names found in the unified structure. This process is also applied to the names of relations and subclasses.

2. **Natural Language Searching:** For searching within the ontology, we utilize a dependency tree to extract the subject, object, and relation from natural language queries. These elements are then used to construct SPARQL queries for simple searches. Additionally, we handle more complex queries by identifying relationships from the dependency tree. For instance, in the query "What is the hyperparameter of mlp and function of it," we identify "hyperparameter" and "function" as related to the "mlp" algorithm, with "hyperparameter" representing the first relation and "function" representing the second relation.

## Used Libraries

- **Spacy:** Used for natural language processing and dependency parsing.
- **Owlready2:** Used for ontology manipulation and querying.
- **Scikit-learn:** Utilized for fuzzy set matching and other machine learning tasks.
- **Fuzzywuzzy:** Specifically used for fuzzy string matching.
- **NumPy:** Used for numerical operations and array manipulations.
