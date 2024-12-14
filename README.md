# Description
Joint project (Mining, Learning and Reasoning on Web Graphs, Ecole Polytechnique, 2023) with Paul Vanborre to study the link between medical deserts in France and the prevalence of lung cancer.

Two large tabular databases are used for this study and can be downloaded at the following links:
- https://www.data.gouv.fr/fr/datasets/effectif-de-patients-par-pathologie-sexe-classe-dage-et-territoire-departement-region/
- https://www.data.gouv.fr/fr/datasets/finess-extraction-du-fichier-des-etablissements/#/resources
The first one contains data on all healthcare facilities in France. The second one lists the number of patients for every category of disease in the country.

# Files
- "creation_graphe.ipynb" creates a graph which gives the distances between every patient and every healthcare facility. It uses the information from the two datasets, as well as queries made to the database Wikidata and calls to the API of OpenStreetMap.
- "requetes_et_visualisation.ipynb" uses this graph to extract relevant information for our analysis. Geopandas is used for vizualisation.
- "rapport.pdf" finally analyses the results and details the visualizations made with Neo4j using Cypher queries.

Note: this project (code and report) was written in French for the purpose of the class.
