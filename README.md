# SSVD

We implemented sparse singular value deomposition (SSVD) in the package `biclustering`. In this repository, simulation, an example on real data, code optimization, and a report are included. 

1. Simulation

Generate X as the sum of X_star and noise term where X_star is equal to s multiplied by u and then by v (s, u and v are given). Noise term is generated from the standard normal distribution. For each iteration, apply SSVD on X to obtain singular vectors (u_hat and v_hat). Compare u with u_hat and v with v_hat. Calculate number of zeros, proportion of correctly classified zeros and nonzeros, and misclassification rate. Repeat the procedure for 100 iterations and calculate the mean of the above criteria. 

2. Example of Lung Cancer Data

In this notebook, SSVD is applied to the lung cancer data stored in data.txt. The first three SSVD layers are extracted and plotted. 

3. Code Optimization

JIT and Cython are used to optimize the original pure Python functions. Results are checked and runtime comparison is provided.

4. Implementation of Biclustering via SSVD

This is a PDF report covering summary, description of algorithm, application, and conclusion.   
