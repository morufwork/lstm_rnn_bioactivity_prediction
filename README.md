# LSTM-Based Bioactivity Prediction of Chemical Compounds

# Project Overview
This project leverages Long Short-Term Memory (LSTM) Recurrent Neural Networks (RNNs) to predict the bioactivity of chemical compounds targeting acetylcholinesterase (AChE)—a key enzyme involved in Alzheimer's disease therapy. Unlike traditional cheminformatics approaches that rely on molecular fingerprint descriptors, our model learns representations directly from SMILES strings, allowing for more flexibility and reduced need for manual feature engineering.

## 🔍 Key Features

- 🧪 **Dataset of 4,620 compounds** from the [ChEMBL](https://www.ebi.ac.uk/chembl/) database  
- 🔬 **Evaluated on 1,000 unlabeled compounds** from [ZINC-20](https://zinc.docking.org/)  
- 🧠 **Sequence-based learning** via character-level SMILES tokenization  
- 📈 **Model trained** using binary cross-entropy loss and optimized with the Adam algorithm  
- ✅ **Performance**: 83% accuracy, 84% precision, 83% recall, 83% F1 score, and 92% AUC  
- 🧠 **SHAP analysis** applied to interpret token-level contributions and model decisions

## 💡 Motivation

Cheminformatics often struggles with:

- 🔬 **Complexity in molecular structures**
- 📉 **Limited domain-specific expertise for feature crafting**

This project addresses these challenges using **deep learning** to autonomously learn chemical representations directly from data, minimizing the need for manual feature engineering.

## 🧪 Dataset

- **Training Data**: 4,620 labeled compounds from [ChEMBL](https://www.ebi.ac.uk/chembl/)
- **Test Data**: 1,000 randomly selected compounds from [ZINC-20](https://zinc.docking.org/)

## 🧠 Model Architecture

- **Input**: Tokenized SMILES strings
- **Embedding Layer**
- **LSTM Layers**
- **Dense Output Layer** (Sigmoid activation)


## 🔬 Model Interpretability

**SHAP (SHapley Additive exPlanations)** was used to interpret model predictions. Key insights include:

- 🧬 **Aliphatic (`"C"`) and aromatic carbon (`"c"`) atoms** were identified as top positive contributors to predicted bioactivity.
- 📊 The model's learned patterns align with **established structure-activity relationships** in medicinal chemistry, increasing confidence in prediction reliability.




## 💡 Applications

- 💊 **Drug discovery and virtual screening**
- 🧬 **Interpretability in cheminformatics**
- 📚 **Educational demos for deep learning in bioinformatics**
