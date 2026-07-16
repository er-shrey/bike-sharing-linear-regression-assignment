# Bike Sharing Demand Analysis (Linear Regression Assignment)

A linear regression assignment modeling daily bike-share demand for a US bike-sharing provider (BoomBikes). The goal is to identify which factors (weather, season, working day, etc.) significantly affect the number of bikes rented per day, so the business can plan for demand recovery post-pandemic.

## Business Goal

Model shared-bike demand (`cnt`) against the available independent variables so management can understand how demand varies with different features and plan business strategy accordingly.

## Tech Stack

- Python 3.9.19
- Jupyter Lab v4.1.6
- pandas, numpy, matplotlib, seaborn
- scikit-learn, statsmodels

## Prerequisites

- Python 3.9+ and pip

## Installation

```bash
pip install jupyterlab pandas numpy matplotlib seaborn scikit-learn statsmodels
```

## Running

```bash
jupyter lab
```

Then open `Shrey_Kumar_jain_bike-sharing-linear-regression-assignment.ipynb` and run all cells. The notebook reads `day.csv` (documented in `Data Dictionary.txt`) from the repo root.

## Project Structure

```
day.csv                                            Daily bike-sharing dataset
Data Dictionary.txt                                 Field descriptions for day.csv
Shrey_Kumar_jain_bike-sharing-linear-regression-assignment.ipynb   Main analysis notebook
Linear+Regression+Subjective+Answers.docx/.pdf      Written answers to subjective questions
```

## Conclusions

Final fitted equation for bike demand (`cnt`), from the multiple linear regression model:

```
cnt = 0.53*temp + 0.23*yr + 0.13*winter + 0.13*Sep + 0.1*summer + 0.06*Aug
      + 0.05*Saturday + 0.04*workingday + 0.04*Oct - 0.06*holiday - 0.06*Mist
      - 0.17*hum - 0.19*windspeed - 0.25*Light + 0.19
```

## Acknowledgements

- UpGrad and IIIT-B faculty

## Contact

Created by [@er-shrey](https://github.com/er-shrey)
