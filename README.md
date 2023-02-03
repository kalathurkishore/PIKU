# CVRP2D
## Overview
This repository contains the code and the data of the paper: CVRP2D: Optimized Route Navigation Considering Vehicle
Capacity for Pickup-Delivery

Submitted for the publication in KDD'23. Below steps can be followed for Execution and Reproducing of the results.

## Running the Code
First unzip the `data.zip` as shown below 
```
unzip data.zip
```
Installing the required packages by 
```
pip3 install -r requirements.txt
```
Acquire Gurobi license
```
https://www.gurobi.com/downloads/free-academic-license/
```
For reproducing the results run `Markov_Approach` as shown below
```
python3 Markov_Approach.py
```
For reproducing the results run `Neural_Network_Approach` as shown below
```
python3 Neural_Network_Approach.py
```
For reproducing the results run `Decision_Focused_Learning_Approach` as shown below
```
python3 Decision_Focused_Learning_Approach.py
```
For reproducing the plots run `VRPSPD_Capacitated_plotting` accordingly based on required capacity where values were obtained from `SPD.py`
