# Estimating Rate of Growth of SARS-CoV-2 in the European Population

## Overview

This project focuses on estimating the growth rate of the SARS-CoV-2 virus in the European population using genetic data analysis. The goal is to identify the parameter responsible for observed genetic changes.


## Methodology

### Data Preparation

- Read and format observation and simulation files.
- Simulations consist of 10,000 datasets with 50 sequences each.

### Pairwise Difference Calculation

- Calculate the average number of pairwise differences between sequences.
- Optimize performance using Rcpp-based C++ implementation.

### Parameter Estimation

#### Average Number of Pairwise Differences (k Estimate)

- `k_estimate` function calculates average pairwise differences for simulations.

#### Rcpp Implementation for Performance

- Utilize C++ with Rcpp to enhance performance.

#### Calculation of Other Parameters

- Calculate "w" and "Tajima's D" based on average pairwise differences.

### Normalization of Parameters

- Normalize parameters for simulations and observations.

### Parameter Comparison and Approximation

- Compare parameters between simulations and observations.

#### Parameter Association

- Associate parameters with distances.
- Select the 500 closest parameters from simulations.

#### Parameter Estimation

- Approximate the parameter that generated the observed dataset based on the 500 closest parameters.

## Results

- The estimated growth rate parameter for SARS-CoV-2 in the European population is approximately 98.4.
- Compared to the mean parameter value of 185.5 from simulations, this suggests a decrease in the virus's growth rate over time.

## Conclusion

This project provides insights into the growth rate of SARS-CoV-2 in the European population using genetic data analysis. The estimation indicates a decrease in the growth rate, which may have implications for understanding the virus's evolution and spread.

## Author

- [Nikolaos Barmparousis](https://github.com/nikbarb810)

## License

This project is licensed under the [MIT License](LICENSE).
