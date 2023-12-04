# Ensemble Kalman Filters with Resampling
This repository contains codes to reproduce all the data and figures presented in 'Ensemble Kalman Filters with Resampling' by Omar Al-Ghattas, Jiajun Bao, and Daniel Sanz-Alonso.

## Paper Abstract
Filtering is concerned with online estimation of the state of a dynamical system from partial and noisy observations. In applications where the state of the system is high dimensional, ensemble Kalman filters are often the method of choice. These algorithms rely on an ensemble of interacting particles to sequentially estimate the state as new observations become available. Despite the practical success of ensemble Kalman filters, theoretical understanding is hindered by the intricate dependence structure of the interacting particles. This paper investigates ensemble Kalman filters that incorporate an additional resampling step to break the dependency between particles. The new algorithm is amenable to a theoretical analysis that extends and improves upon those available for filters without resampling, while also performing well in numerical examples.

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
