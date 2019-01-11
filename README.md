# BBB-Models

This repository contains all Data, Models and Scripts accompanying the manuscript:

Predicting Blood-Brain Barrier Permeability of Marine-Derived Kinase Inhibitors Using Ensemble Classifiers Reveals Potential Leads for Neurodegenerative Disorders. Fabien Plisson and Andrew M. Piggott. Marine Drugs. January 2019. 

## Description

* Data: 
   * _datasetsCompounds.xlsx_ contains all original 968 SMILES of CNS-penetrant small molecules, kinase drugs and marine-derived kinase inhibitors.
   * _datasetsDescrs.csv_, _datasetsNormalizedDescrs.csv_ and _datasetsMorganFingerprints.csv_ contain either calculated 200 (normalized) physicochemical descriptors or Morgan fingerprints from all 968 chemical structures.
   * _logBBvalues.csv_ logBB values for 332 CNS-penetrant small molecules.
   * _similarity_matrix_... Matrices of similarity measurements between all 968 structures using different fingerprints (Atom Pairs, MACCS Keys, Topological, Topological Torsions)
   * _mahanalobis_distance_modelset_ and _mahanalobis_distance_holdoutset.csv_ contain all calculated Mahanalobis distances calculated for all 968 structures (model and holdout sets)
   * _predictions_modelset.csv_ and _predictions_holdoutset.csv_ contain all predicted class membership (0 BBB-, 1 BBB+) and their probability estimates for all 968 structures (model and holdout sets) from our top 3 models (RFC, GBC, LOGREG).

* Scripts: 
   * _1_Data_Preparation_ (Python 3.6)
   * _2_Exploratory_Data_Analysis_ (R, Python 3.6)
   * _3_Models_... (Python 3.6)
   * _4_Predictions_Holdoutset (Python 3.6)

- Models:
Pickled files of our top 3 models (RFC, GBC, LOGREG).
