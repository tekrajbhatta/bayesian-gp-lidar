# bayesian-gp-lidar

## Short description
Bayesian Linear Regression and Gaussian Process Regression on the LIDAR dataset with PyMC and scikit-learn.

## README

# Bayesian Regression and Gaussian Process Regression on the LIDAR Dataset

A personal machine learning practice project exploring Bayesian Linear Regression and Gaussian Process Regression on the LIDAR dataset. The notebook uses PyMC for Bayesian inference and scikit-learn for Gaussian Process regression, and it also compares RBF and Matérn 3/2 kernels on the same data.

## What is included

- Bayesian Linear Regression on a random 100-point subsample of the LIDAR data.
- Gaussian Process Regression on the full dataset with train/test splits.
- Kernel comparison between Squared Exponential (RBF) and Matérn 3/2.
- Additional GP experiments on synthetic functions.

## Dataset

The notebook uses the `lidar.csv` dataset with 221 observations and two columns: `range` and `logratio`.

## Methods

- Bayesian Linear Regression with priors on the intercept, slope, and noise standard deviation.
- Gaussian Process Regression with optimized kernels and predictive intervals.
- Model comparison using test RMSE and log marginal likelihood.

## Repository structure

```text
.
├── bayesian-gp-lidar.ipynb
├── lidar.csv
├── README.md
└── requirements.txt
```

## Getting started

1. Clone the repository.
2. Install the dependencies.
3. Open the notebook and run the cells in order.

## Requirements

- Python 3.10+
- numpy
- pandas
- matplotlib
- scikit-learn
- pymc
- arviz

## Results summary

- Bayesian Linear Regression was fit on a 100-point sample from the LIDAR data.
- GP regression produced similar RMSE values for the 80:20 and 70:30 splits.
- The notebook also compares the behavior of RBF and Matérn 3/2 kernels on the LIDAR dataset.

## License

Repository created for educational purposes.
