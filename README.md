# MSEM-PE6013-Group7Project
# Singapore Bus Network Operations Management Analysis and ILP Optimization  

This notebook uses the Singapore bus dataset to perform an **Operations Management (OM)** analysis and a **linear programming (LP)** optimization model.  

## Objectives
1. Understand the network structure and service characteristics.  
2. Apply OM concepts such as **process analysis, capacity, bottleneck, utilization, and waste identification**.  
3. Build a runnable **ILP model** to allocate additional weekday departures under a limited bus-hour budget.  

> Dataset source : Kaggle - Singapore Bus Data (Land Transport Authority)


## Operations Management Interpretation

### 1. Process analysis
A bus route can be treated as a service process:  
**dispatch → travel → stop servicing → arrival → turnaround**  

### 2. Capacity
For a route, capacity is constrained by:
- service span
- headway
- trip time

### 3. Bottleneck
Potential bottlenecks are routes with:
- long one-way trip time
- many stops
- relatively infrequent weekday service

### 4. Lean waste
Possible wastes include:
- waiting
- unnecessary route overlap
- uneven workload (Mura)
- overburden (Muri) on long routes
