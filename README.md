# KG-OLAP-QG

## Description
Our proposed methodology consists of three main steps: graph generation, pathway exploration, and diverse query generation. \textbf{Figure 2} shows the pipeline of our proposed method. In the graph generation step, we generate the central graph and multi-hop graphs from each surface of the graph cube, treating each graph as an individual surface. Moving on to the pathway exploration step, we perform random walks on each graph to generate different entities. Subsequently, we apply the Dynamic Prompt algorithm, utilizing the entities generated in the previous step, to generate diverse prompts from each graph. Finally, we aggregate all the generated prompts, embed them together, and apply a transformer-based method to generate combined queries based on the different input graphs. To ensure diverse perspectives and comprehensive coverage of node connections within the graphs, we employ beam search on the generated queries.

<p align="center">
   
<img src="https://github.com/mahdieh1/KG-OLAP-QG/blob/main/Images/pipeline.jpg" alt="Pipeline">
</p>

## Table of Contents
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)
- [Contributing](#contributing)
- [Contact](#contact)

## Requirements
- Python (>=3.6)

Install Dependencies: Make sure you have all the required dependencies installed. You can find the list of dependencies in the requirements.txt file. Install them using pip:

```bash
pip install -r requirements.txt
```


## Installation
1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/mahdieh1/KG-OLAP-QG.git
   
## Usage
To use the code and reproduce the results of the paper, follow these steps:

Run Dataset 1:

```bash
python run_dataset1.py

This command will process Dataset 1 and generate the corresponding graphs based on specific features.

Run Dataset 2:

```bash
python run_dataset2.py

Similarly, this command will process Dataset 2 and generate the relevant graphs.

Please note that our code is optimized for these two datasets. For other datasets, some modifications or adaptations may be required. Additionally, feel free to explore the code and adapt it to suit your specific use case.

*Disclaimer: Please make sure to respect the licenses and terms of use associated with Dataset 1 and Dataset 2. These datasets may have specific usage restrictions that you need to be aware of

## License
This project is licensed under the [License Name] License - see the LICENSE file for details.

## Contributing
We welcome contributions to improve the code and methodology. To contribute, please follow these steps:

Fork the repository.
Create a new branch.
Make your changes and commit them.
Push the changes to your forked repository.
Create a pull request with a detailed description of your changes.

## Contact
If you have any questions or feedback, please feel free to contact the authors:
Mahdieh Labani (mahdieh.labani@gmail.com)
