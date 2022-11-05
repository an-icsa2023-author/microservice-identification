# From monolithic to microservice architecture: an automated approach based on graph clustering and combinatorial optimization

## Analysis step

```1-System_analysis.ipynb```

#### Input
Java code

#### Required user information
Refinement of the automated identification of methods, entities and system's layers

#### Ouptuts
- Refinement information file needed for further analysis without further refinements (```[project-name]_refinement.json```)
- Nodes csv file (```[project-name]_nodes.csv```)
- Full edges csv file, without mapping with node keys (```[project-name]_edges_written.csv```)
- Edges csv file, only with references with node keys (```[project-name]_edges.csv```)
- Graph gml file without weights (```[project-name]_graph.gml```)
- Graph png file (```[project-name]_graph.png```)


## Decomposition step

```2-Decomposition_optimization.ipynb```

#### Input
- Graph gml file (```[project-name]_graph.gml```)

#### Outputs
- LP formulation (```[project-name]_communities_improved_optimization.lp```)
- Solution csv file, mapping nodes to microservices (```[project-name]_sol_communities_improved_optimization.csv```)
- Solution image (```[project-name]_sol_communities_improved_optimization.png```)
- Solution analysis (```[project-name]_sol_communities_improved_optimization.txt```)


## Required external packages
- Networkx (https://networkx.org)
- Pygraphviz (https://pygraphviz.github.io)
- Gurobi (https://www.gurobi.com)
- Python-Louvain (https://github.com/taynaud/python-louvain)
- Ipywidgets (https://github.com/jupyter-widgets/ipywidgets)
