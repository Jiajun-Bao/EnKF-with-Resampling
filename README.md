# Ensemble Kalman Filters with Resampling
This repository contains codes to reproduce all the data and figures presented in 'Ensemble Kalman Filters with Resampling' by O. Al Ghattas, J. Bao, and D. Sanz-Alonso.

## Paper Abstract
Filtering is concerned with online estimation of the state of a dynamical system from partial and noisy observations. In applications where the state of the system is high dimensional, ensemble Kalman filters are often the method of choice. These algorithms rely on an ensemble of interacting particles to sequentially estimate the state as new observations become available. Despite the practical success of ensemble Kalman filters, theoretical understanding is hindered by the intricate correlations between the interacting particles. This paper investigates ensemble Kalman filters that incorporate a resampling to break these correlations. 
For the resulting algorithms, we establish theoretical guarantees that extend and improve those available for filters without resampling. Additionally, we numerically show that filters with resampling achieve competitive performance in a partially-observed Lorenz 96 system widely used to test filtering algorithms.

## Repository Contents
This repository consists of three Jupyter notebooks, organized to correspond with sections of the associated paper:
- Linear.ipynb: Notebook for Section 4.1 in the paper 
- L96-main.ipynb Notebook for Section 4.2 in the paper 
- L96-comparison.ipynb: Notebook for addressing the discussion in Algorithm 3.1, specifically the possibility of breaking particle correlations by resampling between forecast and analysis steps. While this approach would be amenable to a non-asymptotic analysis akin to the one we develop, we empirically found that resampling after the forecast step significantly deteriorates the performance of the filter in nonlinear settings. 

## Environment Details
For the computations, the following environment was used:
- Python version:  3.9.12
- Numpy version:  1.21.5
- Scipy version:  1.7.3
- Matplotlib version:  3.5.1
- OS info:  10.16 (x86_64)
- CPU cores:  8
