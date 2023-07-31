# KG-OLAP-QG

## Description
Our proposed methodology consists of three main steps: graph generation, pathway exploration, and diverse query generation. \textbf{Figure 2} shows the pipeline of our proposed method. In the graph generation step, we generate the central graph and multi-hop graphs from each surface of the graph cube, treating each graph as an individual surface. Moving on to the pathway exploration step, we perform random walks on each graph to generate different entities. Subsequently, we apply the Dynamic Prompt algorithm, utilizing the entities generated in the previous step, to generate diverse prompts from each graph. Finally, we aggregate all the generated prompts, embed them together, and apply a transformer-based method to generate combined queries based on the different input graphs. To ensure diverse perspectives and comprehensive coverage of node connections within the graphs, we employ beam search on the generated queries.\\

![Alt Text](https://github.com/mahdieh1/KG-OLAP-QG/blob/main/Images/pipeline.jpg)

## Table of Contents
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Methodology Overview](#methodology-overview)
- [Code Structure](#code-structure)
- [License](#license)
- [Contributing](#contributing)
- [Contact](#contact)

## Requirements
- Python (>=3.6)


## Installation
1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/mahdieh1/your_repository.git
Usage
To use the code and reproduce the results of the paper, follow these steps:

(Add any specific data preprocessing steps, if applicable.)
(Provide details on how to run the main code or any specific scripts.)
Methodology Overview
Our proposed methodology consists of three main steps:

Graph Generation:
The graph generation step involves creating the central graph and multi-hop graphs from each surface of the graph cube, treating each graph as an individual surface. (Add more details about the specific graph generation algorithm used.)

Pathway Exploration:
In the pathway exploration step, we perform random walks on each graph to generate different entities. (Provide more information about the random walk strategy and its importance in the methodology.)

Diverse Query Generation:
The diverse query generation step employs the Dynamic Prompt algorithm, utilizing the entities generated in the previous step, to generate diverse prompts from each graph. We then aggregate all the generated prompts, embed them together, and apply a transformer-based method to generate combined queries based on the different input graphs. To ensure diverse perspectives and comprehensive coverage of node connections within the graphs, we employ beam search on the generated queries. (Include more details on the Dynamic Prompt algorithm and the transformer-based method.)

Figure 1 shows the pipeline of our proposed method.

Code Structure
The repository is organized as follows:

main.py: The main script for executing the methodology.
graph_generation.py: Contains functions related to graph generation.
pathway_exploration.py: Contains functions for pathway exploration using random walks.
diverse_query_generation.py: Implements the diverse query generation using the Dynamic Prompt algorithm and transformer-based method.
utils.py: Utility functions used throughout the code.
data/: Directory containing any necessary data files or datasets.
(Add more details about the code structure, such as dependencies, and any other important files.)

License
This project is licensed under the [License Name] License - see the LICENSE file for details.

Contributing
We welcome contributions to improve the code and methodology. To contribute, please follow these steps:

Fork the repository.
Create a new branch.
Make your changes and commit them.
Push the changes to your forked repository.
Create a pull request with a detailed description of your changes.
Contact
If you have any questions or feedback, please feel free to contact the authors:

Author Name (author@email.com)
