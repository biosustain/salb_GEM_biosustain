# Salb-GEM-v1.1(Biosustain): Genome-scale metabolic model of _Streptomyces albus_ J1074


## Description  
Salb-GEM-v1.1(Biosustain) is a genome-scale metabolic model (GEM) reconstructed for **_Streptomyces albus_ J1074**, based on original version of Salb-GEM and phenomics data from [DTU Biosustain](https://www.biosustain.dtu.dk/). This model enables in silico simulations of metabolic fluxes under diverse conditions, supporting applications in:  
- 🧬 **Systems biology** (multi-omics integration, phenotype prediction)  
- 🧪 **Biotechnology** (strain engineering, substrate utilization)  
- 🧠 **Basic research** (gene essentiality, metabolic pathway analysis)  


## Citation  


## Model Overview  
| Property               | Value       | Description                                  |  
|------------------------|-------------|----------------------------------------------|  
| **Taxonomy**           | [salb](https://www.genome.jp/dbget-bin/www_bget?gn:salb)   |  _Streptomyces albus_ J1074                     |  
| **Latest Update**      | 2025-07-13  |                       |  
| **Version**            | 1.1       |                        |  
| **Reactions**          | 2274       |                   |  
| **Metabolites**        | 1888       |                              |  
| **Genes**              | 1405       |               |  



## Installation & Usage  
### Obtaining the Model  
```bash  
git clone https://github.com/biosustain/Salb-GEM-Biosustain.git
```

### Python (cobrapy):
```python
from cobra.io import load_json_model  
model = load_json_model("./model/Salb-GEM-v1.1(Biosustain).json")  
```

## Model Files
```
root
├── model
│   └── Salb-GEM-Biosustain.xml: The metabolic model in SBML format
│   └── Salb-GEM-Biosustain.yml: The metabolic model in YAML format
│   └── Salb-GEM-Biosustain.json: The metabolic model in JSON format
│   └── Salb-GEM-Biosustain.mat: The metabolic model in MatLab format
└── notebooks: Model curation workflow
│   └── 1.phenomics: Create evaluation metrics using phenomics data
│   └── 2.gapfilling: Gapfill Salb-GEM model using various gapfilling techniques
│   └── 3.pathway_engineering: Engineer PTA pathway into the gapfilled Salb-GEM
│   └── 4.medium_optimization: Using engineered PTA pathway model for medium optimization
│   └── 5.paper: Figure creation for publication
└── data:  External Data used for gapfilling and manual curation
│   └── external: Genomics scale models and name matching files for gapfilling
│   └── interim: Files generated from gapfilling
│   └── raw: Pheomics and fermentation data
```

## Validation
The model has been validated against:

## Version History
All model releases will be archived on Zenodo.

## Contributing
Contributions are welcome! Please read our contributing guidelines before submitting issues or pull requests.

## Related Models
- [Salb-GEM](https://github.com/SysBioChalmers/Salb-GEM)
- [Sco-GEM](https://github.com/SysBioChalmers/Sco-GEM)
- [Vene-GEM](https://analyticalsciencejournals.onlinelibrary.wiley.com/doi/10.1002/bit.28114)

## Contact
- [Te Chen](https://orbit.dtu.dk/en/persons/te-chen)
- [The Novo Nordisk Foundation for Biosustainability, Technical University of Denmark](https://www.biosustain.dtu.dk/)

## Acknowledgments
<img src="https://upload.wikimedia.org/wikipedia/commons/4/48/Novo_Nordisk_Foundation_logo.svg" alt="NNF" style="height: 100px;"/>
Quantitative Modelling of Cell Metabolism
Keywords: genome-scale metabolic model, systems biology, Streptomyces, metabolic engineering, flux balance analysis

## License
![MIT](https://img.shields.io/badge/License-MIT-blue.svg)
