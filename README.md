# Demystifying catalytic CO<sub>2</sub> reduction pathways with thousands of elementary reactions via mechanism discovery and machine-learned kinetic barriers

**Abstract**: <br>
Heterogeneous catalytic pathways involve thousands of elementary steps, forming an
 intricate web of chemical reactions, but most first-principles kinetic models involve only
 a few dozen elementary steps. Here, we combine extensive quantum-mechanical cal
culations of reaction thermodynamics/kinetics, machine-learning models for activation
 barrier prediction, and methods for automated reaction enumeration and elementary re
action identification. Thereby, we devise an approach that enables automated microki
netic modeling (MKM) of CO<sub>2</sub> reduction pathways on copper with an unprecedented
 9389 elementary reactions. We validate our computational outcomes with experimen
tal observations. The ensuing results follow experimental trends of methanol and CO
 production rates, contrary to the conclusions of MKM based on a smaller subset of
 manually curated reactions. Considering hundred-plus C1-C4 compounds, our auto
mated approach unravels intermolecular hydrogen-hopping reactions to be the key to
 accurately simulating the CO<sub>2</sub> reduction pathway. We also establish the importance
 of CH<sub>3</sub>CHO in forming longer-chain hydrocarbons. Overall, the proposed strategy to
 comprehensively model complex catalytic pathways will significantly advance compu
tational catalysis research and carbon conversion processes.
<br>
<br>

![Cover Image](https://github.com/agrgroup/Thermochemical-CO2RR/assets/70911775/1aeebc54-3206-4308-a1b8-fef90d46ae1a)

This project is organized into multiple folders, each containing relevant notebooks and data files for various machine learning models and frameworks. Below is an overview of the directory structure, including descriptions of each file and its purpose.

## Directory Structure:
### ML: 
This folder contains files related to the AE-RE and AFE-RFE models, along with their implementations.

#### Ea.ipynb:
This notebook implements feature engineering, hyperparameter tuning, model selection, and prediction for the AE-RE model.

#### Ga.ipynb:
This notebook implements feature engineering, hyperparameter tuning, model selection, and prediction for the AFE-RFE model.

#### Prediction.ipynb:
This notebook provides an end-to-end prediction workflow from the AE-RE model to the AFE-RFE model.

#### LOOCV.ipynb:
This notebook implements Leave One Out Cross-validation for the AE-RE model.

#### kfCV.ipynb:
This notebook implements k-Fold Cross-validation for the AFE-RFE model.

Feel free to explore each notebook for detailed implementations and methodologies!

### ERI: 
This folder contains files related to the ERI framework.

#### ARE Ouput (ERI Input).csv:
Input file for ERI containing all the reactions generated from ARE.

#### Benchmark_elementary_reactions.csv:
This csv file contains manually labelled reactions used to validate the ERI framework.

#### Elementary_Reaction_Identifier.ipynb:
This notebook implements the ERI framework.

### ARE:

#### Automated Reaction Enumeration.ipynb
Code to enumerate all possible reactions based on intermediates provided.

#### ads species(ARE input file)
Input file for containing intermediates information

#### ARE Ouput (ERI Input).csv:
Input file for ERI containing all the reactions generated from ARE.




