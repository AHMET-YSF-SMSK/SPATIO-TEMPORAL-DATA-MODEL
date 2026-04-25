# This repo have for LSM-GNN hybrid deep learning algorithms data creator model
LSM-GNN Hybrid Deep Learning Data Generator
Overview
This repository provides a modular driving record data generation model designed for LSM-GNN (Long Short-Term Memory & Graph Neural Network) hybrid deep learning algorithms. It dynamically generates both spatial (real-world road networks) and temporal (physics-based travel time) data.

Tech Stack

Python

OSMnx (Spatial data extraction and network routing)
 networkx
pandas
numpy
torch
from torch_geometric.utils from_networkx
from sklearn.model_selection train_test_split

Key Features

Modular Spatial Generation: Extracts real-world road networks. Users only need to specify the origin, desired intermediate points and destination coordinates. (Co-developed with @Rumeyssayslv).

Temporal Synthesis: Generates realistic travel time data based on the spatially captured routes using physics principles, Markov diagrams, Traffic rules(Türkiye for maxspeed).It also generates nine different types of anomalies, including GPS and user anomalies.

Current Status & Known Issues (WIP)
Very large changes in the maximum speed limit in the road data sometimes cause a recurrence limit error. Although some code blocks have been added to resolve this issue, the problem still persists.
Currently, the "stop at traffic light" function is under development and its addition is being discussed. Other than that, there are no other missing features.
