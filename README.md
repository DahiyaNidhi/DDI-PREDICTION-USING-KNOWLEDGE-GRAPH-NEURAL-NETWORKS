# Drug-Drug Interaction Prediction using Knowledge Graph Neural Networks

## Overview

This project leverages Knowledge Graph Neural Networks (KGNNs) to predict potential Drug-Drug Interactions (DDIs) using structured biomedical data. Built on a model inspired by Lin et al. (IJCAI 2020), it uses data from DrugBank to train a multi-relational graph model for accurate DDI prediction. The system is designed for scalability and can support future drug safety research.

## Key Features

- **Model**: Knowledge Graph Neural Network (KGNN) with multi-hop neighborhood aggregation
- **Dataset**: Parsed DrugBank XML to create a biomedical Knowledge Graph with drugs, proteins, and interactions
- **Metrics**: AUC: 0.9323, AUPR: 0.9132, F1-Score: 0.892
- **Negative Sampling**: Random negative DDI pair generation to balance dataset
- **Framework**: Implemented using TensorFlow/Keras with modular pipeline

## How It Works

1. **Build the Graph**: Extract entities (drugs, proteins) and relations from DrugBank to construct a Knowledge Graph
2. **Train the Model**: Learn drug embeddings using KGNN, trained on known DDI pairs
3. **Make Predictions**: Predict unseen DDIs and evaluate performance using AUC, AUPR, and F1 metrics
4. **Interpret Results**: Analyze interaction predictions to support drug safety evaluations and pharmaceutical research
