# ReTiNA-1: Automated LC-MS Retention Time Modeling

ReTiNA-1 is a large open-source dataset and collection of machine learning models in active development for predicting small molecule retention times in LC-MS workflows.

## ⚗️ The ReTiNA-1 Dataset

The ReTiNA-1 dataset contains:

- 4,359,188 unique molecule–environment combinations, the largest singular LC-MS retention time dataset of its kind to date
- Experimentally measured retention times, in seconds, curated from public datasets, benchmark papers, and literature

The dataset is actively expanding with new experimental retention time values from the Coley Research Group at MIT, ensuring it remains a growing resource for optical property prediction.

Additionally, ReTiNA-1 includes ```.smi``` lists of 641,651 unique compounds and 6 unique solvents in the dataset for chemical descriptor calculations.

91 distinct LC-MS setup environments are used in ReTiNA-1. Each environment consists of:

- Solvent mixtures A and B, consisting of solvents and solvent additives contributing to pH
- The mobile phase gradient used, defined by the percentage of solvent mixture B over time (min)
- The chromatographic technique used - either HILIC or reverse phase 
- LC-MS column dimensions, in terms of column length (mm), internal diameter (mm), and particle size (µm)
- The mobile phase flow rate, measured in mL/min
- The column temperature, measured in degrees Celsius

The full dataset is accessible at this [Hugging Face Repository](https://huggingface.co/datasets/natelgrw/ReTiNA-1).

ReTiNA-1 is designed for use in:

- Estimating retention times for new compound–environment combinations
- Aiding in peak assignment during LC-MS method development
- Training ML models for retention time prediction under specific conditions

## 📋 Data Sources Used

Detailed information on the data sources comprising the ReTiNA-1 dataset can be found in the the Hugging Face repository linked above.

## ✒️ Citation

If you use the ReTiNA-1 dataset in a project, please cite the following:

```
@dataset{natelgrwretina1dataset,
  title={ReTiNA-1: A Benchmark Dataset for LC-MS Retention Time Modeling},
  author={Leung, Nathan},
  institution={Coley Research Group @ MIT}
  year={2025},
  howpublished={\url{https://huggingface.co/datasets/natelgrw/ReTiNA-1}}
}
```
