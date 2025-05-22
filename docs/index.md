# Enhancing Secure Multi-Party Computation with Damgård-Jurik and NIZK

Privacy preserving secure multi party computation protocols are known to face scalability and efficiency challenges in environments where participants hold distinct attributes of the same records (vertical partitioning) or controls a subset of complete records (horizontal partitioning), as in cross-institutional health data analysis or federated IoT analytics, mostly because of communication overhead and the need to address adaptability to large scale or heterogeneous settings. We present a secure sum protocol based on the 
Damgård-Jurik cryptosystem, implemented and evaluated within an experimental setup that considers both vertical and horizontal partitioning. The proposed protocol exploits its additive homomorphic properties to enable efficient aggregation with a single encryption 
round per party, hence significantly reducing computational and communication costs, while ensuring privacy and integrity via encryption and Non-Interactive Zero-Knowledge Proofs (NIZK). Furthermore, the practical feasibility of this protocol is reinforced by proof-of-concept and performance evaluation, demonstrating its effectiveness and efficiency in handling large datasets.


## Requirements

- one virtual machine (VM) for each node
- virtual enviroment for each VM
- Allow root privileges to install libreries

## Instructions

1. Activate virtual enviroment

Step 1:
```bash
 python3 -m venv .venv
```
Step 2:
```bash
source .venv/bin/activate
```

2. Install necessary libraries 

Step 1: 
```bash
pip install zmq sympy pandas
```


## Demo
The demonstration is given of how to expand the proposed protocol to 4 participating nodes.

- [Mehnaz Example](Mehnaz.zip)
- [Proposed Genmeralization](Proposed_Generalization.zip)


## Metrics

The files with the metrics associated with the experiments performed are:

1. [Execution Times - Horizontal Partition](Execution_Times-Horizontal_Partition.xlsx)
2. [Execution Times - Vertical Partition](Execution_Times-Vertical_Partition.xlsx)
