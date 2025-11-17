# DSC212 – Modularity on the Karate Club Graph
### Recursive Spectral Community Detection & Network Metrics

This repository contains the full implementation of the **DSC212 Graph Theory assignment** on **modularity-based community detection** using **spectral bisection** on the classic *Zachary’s Karate Club* network.

---


---

## 🔍 Overview of the Method

### 1. Modularity Matrix Construction
Given adjacency matrix A and degrees kᵢ:

**B = A - (k kᵀ) / (2m)**

This compares observed edges to a degree-preserving random graph.

### 2. Leading Eigenvector Partition
The leading eigenvector u₁ of B:

- Positive entries → Community 1  
- Negative entries → Community 2  

This approximates the optimal solution to maximizing modularity.

### 3. Recursive Bisection
A subcommunity C is split **only if** its restricted modularity matrix has a positive leading eigenvalue:

**λ₁(C) > 0**

Otherwise, no further division improves modularity.

### 4. Network Metrics After Each Split
Computed for each iteration:

- Degree centrality  
- Betweenness centrality  
- Closeness centrality  
- Clustering coefficient  

These are plotted to observe how structural roles evolve during community detection.

---

## 📊 Outputs Produced

- Final community visualization  
- Metric evolution plots  
- Discussion of central nodes and structural patterns  

---


---

## 📚 References

- Newman (2006). *Modularity and community structure in networks*. PNAS 103(23): 8577–8582.  
- Zachary (1977). *An information flow model for conflict and fission in small groups*. Journal of Anthropological Research.
