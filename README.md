# BANA482 | Multiple Regression in Biology & Analytics

Case 5 repository for my multiple regression analysis using the Forest Fires dataset.

I built this repo as a clean, reproducible home for the analysis, report, presentation, and supporting materials. I focus on how environmental and fire-weather variables relate to burned forest area, using `log(area + 1)` as the regression outcome.

## What I Am Analyzing

I use the Forest Fires dataset to study environmental impact through multiple regression. The main response variable is burned area, transformed as `log(area + 1)` because the original `area` values are highly right-skewed.

The analysis includes:

- data understanding and cleaning
- exploratory analysis
- multiple regression modeling
- multicollinearity checks
- diagnostic testing
- candidate model comparison
- train/test validation
- interpretation for environmental and analytics decisions

## Repository Structure

```text
.
|-- .gitattributes
|-- .gitignore
|-- CITATION.cff
|-- LICENSE
|-- README.md
|-- requirements.R
|-- analysis/
|   `-- case5-multiple-regression.Rmd
|-- data/
|   |-- forestfires.csv
|   `-- forestfires.names
|-- presentations/
|   |-- case5-presentation.pdf
|   |-- case5-presentation-v2.pdf
|   `-- editable/
|-- references/
|   `-- case-5-multiple-regression-in-biology-and-analytics.pdf
`-- reports/
    |-- case5-analysis-output.pdf
    |-- case5-multiple-regression-report.pdf
    |-- case5-qa-prep.pdf
    |-- case5-speaker-notes.pdf
    `-- editable/
```

## How I Run the Analysis

I run the main analysis from:

```text
analysis/case5-multiple-regression.Rmd
```

The notebook reads the dataset from `data/forestfires.csv`. It works when I knit it from the `analysis/` folder or when I run it from the repository root.

I install the required R packages with:

```r
source("requirements.R")
```

## Dataset Citation

I use the public Forest Fires dataset created by Paulo Cortez and Anibal Morais.

Please cite:

Cortez, P., and Morais, A. (2007). A Data Mining Approach to Predict Forest Fires using Meteorological Data. In Proceedings of the 13th Portuguese Conference on Artificial Intelligence, pp. 512-523.

## License

I license my analysis, code, and original project materials under the MIT License. The dataset remains credited to its original authors.
