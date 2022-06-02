# Day 2

Day 2 will focus on the concepts needed to understand
modern deep learning in chemistry. We will cover the types
of chemical data, equivariances and other inductive biases,
modern deep learning architectures, and how to choose them.

The learning objectives for day 2 are:

* Categorizing chemical data
* Identify equivariances and other inductive biases in chemical data
* Choose data transforms and architecture for equivariances
* Understand the graph neural network and its update equations
* Basic understanding of sequence learning and geometric learning

On day 2, it's assumed you have covered the content in day 1 or otherwise
have a machine learning background.

## What is a molecule?

* Molecules as a graph
* Molecules as a line notation/string - SMILES, DeepSMILES, BigSMILES, SELFIES, InChi
* Molecules as a point cloud
* Molecules as a probability distribution
* Labels: properties vs atoms
* Other data types - formulation, periodic, etc.
* Cheminformatics intro - drawing, fingerprints, similarity

## Activity 1: Working with Structures

In this activity, we'll work with a set of a few molecules and draw them,
convert them to graphs, compute similarity, and enumerate chemical neighborhoods.

## Symmetry and Equivariances

* What is an inductive bias
* Definition of a group, group relation
* Definition of major symmetries: permutation, rotation, translation, scale
* Treating symmetry with augmentation or data transformations
* Connecting symmetry to data and model

**Break (15 min.)**

## Neural Networks & Equivariances

0. MLP
1. Graph Neural Networks
2. Convolutional neural networks and how to avoid them
3. Sequence Neural Networks (RNN, Transformer)
4. Equivariant Neural Networks
5. Modifications that can depend on task: VAE, NFlow

## Activity 2: Deciding on a Network

Working in a group, decide on inductive biases and network
choice for given datasets:

1. Predicting solubility from SMILES
2. Finding the reactive site on a molecule from SMILES
3. Predicting partial charge from coordinates
4. Predicting electronic density from coordinates

**Break (15 min.)**

## Graph Neural Networks In Depth

* The Kipf & Welling Graph Convolutional Neural Network (GCN)
* Viewing as message passing (MPNN) and SchNet
* Readouts

## Activity 3: Basic GNN

Revisit the solubility task and predict solubility of molecules with a GNN. See [activity here](https://dmol.pub/dl/gnn.html#kipf-welling-gcn)
