# Hypothesis Testing in Healthcare: Drug Safety

## Overview

This project explores and answers critical questions related to drug safety based on a pharmaceutical company's randomized controlled drug trial dataset. The dataset, provided by GlobalXYZ, focuses on adverse effects, demographic data, vital signs, and other relevant information. The primary objective is to determine if the observed adverse reactions, if any, are of significant proportions.

## Dataset

The dataset, originally obtained from Hbiostat courtesy of the Vanderbilt University Department of Biostatistics, has been modified to include information on the presence and absence of adverse effects and the number of adverse effects experienced by individuals.

### Columns:

- **sex:** The gender of the individual
- **age:** The age of the individual
- **week:** The week of the drug testing
- **trx:** The treatment group (Drug) and control group (Placebo)
- **wbc:** The count of white blood cells
- **rbc:** The count of red blood cells
- **adverse_effects:** The presence of at least a single adverse effect
- **num_effects:** The number of adverse effects experienced by a single individual

## Project Instructions

The project involves several key analyses:

1. **Proportion Test:**
   - Utilize the `statsmodels` library to perform a two-sided z-test on the proportions of adverse effects between the Drug and Placebo groups.

2. **Chi-Square Test:**
   - Determine if the variables `num_effects` and `trx` (treatment group) are independent using the chi-square test.

3. **Exploratory Data Analysis:**
   - Visualize the distribution of age in the Drug and Placebo groups using Seaborn.
   - Optionally, conduct a normality test to inform the choice between an unpaired t-test and a Mann-Whitney U test.

4. **Mann-Whitney U Test:**
   - Conduct a two-sided Mann-Whitney U test to compare the ages of the Drug and Placebo groups, considering the non-normal distribution observed.

## Code Structure

- [drug_safety_analysis.ipynb](notebooks/drug_safety_analysis.ipynb): Jupyter Notebook containing the main analysis code.
- [drug_safety.csv](data/drug_safety.csv): Modified dataset for drug safety analysis.
- [LICENSE](LICENSE): MIT License for the project.

