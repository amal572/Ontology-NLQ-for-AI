# Data_mining_project
We have written an algorithm to standardize different ontologies according to the structure provided by the subject teacher this ontology have a lot of XML file continue of the name of the AI algorithm and its relation to it, then searching this ontology using natural language by converting it to SPARQL language.

<li>we loop for all ontology class names and then use the Fuzzy set to find If the names are the same or not then replace this names to the name find in the unified structure and use the same way for the name of the relation and for subclass </li>

<li>then for search, we use a dependency tree to find the subject, object, and relation from the natural language to use it in SPARQL language for simple query
and try to solve some complex queries to find some relation in the relation from the dependency tree, like the sentence "what is the hyperparameter of mlp and function of it" we find the word "hyperparameter" and "function" related to mlp algorithm and this the subject and hyperparameter is the first relation and function is the second relation so we can find the answer for this type of question. </li>

<h2> used libraries </h2>
<li> spacy </li>
<li> owlready2 </li>
<li> sklearn </li>
<li> fuzzywuzzy </li>
<li> numpy </li>



