# Metabolic Syndrome and Severe Tooth Loss in Chilean Adults

Analytical code for the cross-sectional study examining the association 
between metabolic syndrome and tooth loss–related oral health outcomes 
using data from the Chilean National Health Survey (ENS) 2016–2017.

## Authors

- Felipe Williamson Dargham
- Jaime Cerda Lorca
- Amaru Simón Agüero Jiménez
- Daniela Díaz-Catalán *(corresponding author)*
- Manuel Vásquez-Muñoz *(corresponding author)*

## Study Overview

This secondary analysis of the ENS 2016–2017 (n = 3,489) examined 
the association between metabolic syndrome (defined per NCEP ATP III 
criteria) and four oral health outcomes: cavitated caries, nonfunctional 
dentition (<20 teeth), complete edentulism, and denture use. 
Associations were estimated using survey-weighted logistic regression 
adjusted for age, sex, region, area of residence, health insurance, 
and educational attainment.

## Repository Contents

| File | Description |
|------|-------------|
| `index.qmd` | Main Quarto document with full analysis pipeline |
| `index.html` | Rendered HTML output of the analysis |

## Analysis Pipeline

The code covers the following steps:

1. **Data Management and R Packages** — package installation and loading
2. **Methods**
   - Study design and sampling frame description
   - Participant selection (inclusion/exclusion criteria)
   - Variable operationalization (metabolic syndrome components, 
     oral health outcomes, covariates)
   - Survey design object (`svydesign`) accounting for stratification, 
     clustering, and sampling weights
3. **Statistical Analysis**
   - Descriptive analysis (weighted proportions, means, medians)
   - Bivariate analysis (chi-squared tests, crude ORs)
   - Multivariable analysis (hierarchical survey-weighted logistic 
     regression, Models 1–7)
   - Individual MS component analysis
   - Model diagnostics (Hosmer–Lemeshow test, deviance residuals, 
     GVIF for multicollinearity)
   - Sensitivity analysis (excluding participants >65 years)

## Software

- **R** version 4.4.1
- **RStudio** with Quarto
- Key packages: `survey`, `dplyr`, `broom`, `knitr`, `kableExtra`

## Data Availability

The raw data underlying this analysis are derived from the Chilean 
National Health Survey (ENS) 2016–2017, held by the Ministry of Health 
of Chile (MINSAL). These data are not publicly redistributable due to 
institutional restrictions. Access may be requested from MINSAL through 
a formal public transparency petition under Ley de Transparencia 
No. 20.285 (https://www.bcn.cl/leychile/navegar?idNorma=276363).

## License

This code is shared under the [MIT License](LICENSE).

## Citation

If you use this code, please cite the associated manuscript:

> Williamson Dargham F, Cerda Lorca J, Agüero Jiménez A, 
> Díaz-Catalán D, Vásquez-Muñoz M. Metabolic Syndrome and Severe 
> Tooth Loss in Chilean Adults. *Journal of Dental Research*. 2026.
> [DOI pending]
