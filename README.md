# Statistical Consulting Report and Analysis

This repository contains the files and code related to the analysis of preterm rabbit lung aeration experiments, which explore the effects of various ventilation settings on airway resistance during lung aeration. The goal of the project was to identify optimal ventilatory strategies that reduce airway resistance and minimize time to effective respiration.

## Project Overview

### Background

Preterm infants often face challenges in transitioning from liquid-filled lungs to effective gas exchange after birth due to underdeveloped respiratory systems. This study modeled this scenario using preterm rabbits as a proxy to investigate how ventilator settings influence lung aeration and airway resistance.

### Objective

Determine which combinations of ventilatory settings minimize airway resistance.

### Repository Contents

Statistical_Consulting_Report.pdf: Final report detailing methodology, results, and conclusions.

Client_Analysis_Complete.Rmd: R Markdown file containing code and statistical analyses performed in the study.

### Outputs

The analysis results include:

Identification of significant ventilation settings, including:

Target tidal volume: 10 mL/kg

Respiratory rate: 24-30 breaths per minute

Insights from both clustering and mixed-model approaches.

Visualizations of key data relationships and model performance.

Methodology

Experimental Design

Subjects: 105 preterm rabbits delivered via cesarean section.

Data Collection: High-frequency X-ray imaging during the first two minutes of ventilation.

Ventilator Settings: Various combinations of seven parameters, including tidal volume, respiratory rate, PEEP (positive end-expiratory pressure), and surfactant presence.

### Statistical Analysis

K-means Clustering:

Grouped data into clusters based on time to minimal resistance and airway resistance values.

Identified critical settings leading to optimal outcomes.

Bagging (Bootstrap Aggregatiion):

Enhanced model reliability and identified key predictors, such as respiratory rate and tidal volume.

Linear Mixed Models (LMMs):

Incorporated fixed effects (ventilation settings) and random effects (biological variability among siblings).

Addressed data correlation and ensured robust inference.

Usage

### Requirements

The analysis requires R and the following R packages:

tidyverse

lme4

nlme

caret

### Running the Analysis

Clone this repository.

Open the Client_Analysis_Complete.Rmd file in RStudio.

Install the required packages.

Knit the R Markdown file to generate a reproducible report.

## Key Findings

Optimal Settings: A tidal volume of 10 mL/kg and respiratory rates of 24-30 bpm significantly reduced airway resistance and time to minimal resistance.

Robustness of Results: Both machine learning and statistical modeling approaches confirmed these findings, though limitations such as small sample size were noted.

Practical Implications: The identified settings provide guidance for neonatal ventilator configurations to support preterm infants.

### Limitations

Small sample size and unbalanced dataset.

Limited focus on the initial phase of lung aeration.

Lack of long-term health outcome measurements for subjects.

## Contributions

Authors: Levi Duijst & Alexandros Ioannou

Supervisors: Prof. Dr. Hendriek Boshuizen & Dr. Fred van Eeuwijk

License

This project is licensed under the MIT License.

For detailed explanations and methodology, refer to the Statistical_Consulting_Report.pdf. If you have any questions, please open an issue or contact the authors.

