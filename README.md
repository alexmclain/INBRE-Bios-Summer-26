# SC INBRE Biostatistics Summer Course 2026

**Course Presenter:** [Dr. Alexander McLain](https://sc.edu/study/colleges_schools/public_health/faculty-staff/mclain_alexander.php), Professor of Epidemiology and Biostatistics, University of South Carolina Arnold School of Public Health

**Course Website:** [scinbre.org — 2026 Summer Workshop](https://www.scinbre.org/learning/bids-tutorials-and-workshops/2026-summer-workshop)

**Registration:** [Eventbrite — Register by May 22](https://www.eventbrite.com/e/sc-inbre-2026-biostatistics-summer-courses-tickets-1986660762821?aff=oddtdtcreator)

---

## Overview

This repository contains lecture slides, R lab materials, datasets, and supporting code for the SC INBRE 2026 Biostatistics Summer Courses. The course is offered as three independent one-week modules — participants may enroll in any combination.

The course is designed for faculty, graduate students, and advanced undergraduates in the biological and biomedical sciences. No prior programming experience is assumed for Week 1. Each day consists of a two-hour morning lecture and a two-hour afternoon R lab.

**Format:** In-person (USC Columbia, Discovery Building Computing Lab, 915 Greene St., Suite 303B) or virtual

**Daily Schedule:** 9:00–11:00 AM (Lecture) | 1:00–3:00 PM (R Lab)

---

## Repository Structure (tentative)

```
├── week1-foundations/
│   ├── day01-orientation/
│   ├── day02-r-fundamentals/
│   ├── day03-tidyverse/
│   ├── day04-ggplot2/
│   └── day05-inference/
├── week2-statistical-modeling/
│   ├── day06-linear-regression/
│   ├── day07-model-selection/
│   ├── day08-logistic-regression/
│   ├── day09-survival-analysis/
│   └── day10-mixed-models/
├── week3-bioinformatics/
│   ├── day11-genomics-data/
│   ├── day12-differential-expression/
│   ├── day13-multiple-testing/
│   ├── day14-pca-penalized-regression/
│   └── day15-reproducible-research-capstone/
└── data/
```


---

# Tentative Schedule

## Week 1 (June 1–5): Foundations of Data Science in R

*Target: Assumes no prior R experience. All participants working with biological data.*

| Day | Date | Morning Lecture | Afternoon Lab |
|-----|------|----------------|---------------|
| 1 | Mon, June 1 | Course Overview & Orientation to Data Science | Getting Started with R and RStudio |
| 2 | Tue, June 2 | R Programming Fundamentals | Working with Data in R |
| 3 | Wed, June 3 | Data Wrangling with the tidyverse | tidyverse Lab |
| 4 | Thu, June 4 | Data Visualization with ggplot2 | ggplot2 Lab |
| 5 | Fri, June 5 | Probability, Distributions, and Statistical Inference | Simulation & Inference Lab |

**Key packages:** `tidyverse` (`dplyr`, `tidyr`, `ggplot2`, `readr`), `rmarkdown`, `quarto`

---

## Week 2 (June 8–12): Statistical Modeling

*Target: Applied regression methods for quantitative, binary, time-to-event, and clustered outcomes.*

| Day | Date | Morning Lecture | Afternoon Lab |
|-----|------|----------------|---------------|
| 6 | Mon, June 8 | Simple and Multiple Linear Regression | Linear Regression Lab |
| 7 | Tue, June 9 | Model Selection and Variable Importance | Model Selection Lab |
| 8 | Wed, June 10 | Logistic Regression and Binary Outcomes | Logistic Regression Lab |
| 9 | Thu, June 11 | Survival Analysis | Survival Analysis Lab |
| 10 | Fri, June 12 | Mixed Models and Clustered/Repeated Data | Mixed Models Lab |

**Key packages:** `lm`/`glm` (base R), `pROC`, `survival`, `survminer`, `lme4`, `caret`/`rsample`

---

## Week 3 (June 15–19): Bioinformatics & High-Dimensional Data

*Target: Genomics workflows, dimensionality reduction, penalized regression, and reproducible reporting.*

| Day | Date | Morning Lecture | Afternoon Lab |
|-----|------|----------------|---------------|
| 11 | Mon, June 15 | Genomics Data: Structure, Formats, and Public Databases | Accessing Public Genomics Data |
| 12 | Tue, June 16 | Differential Expression Analysis | DESeq2 Lab |
| 13 | Wed, June 17 | Multiple Testing, FDR, and Visualization | Multiple Testing & Visualization Lab |
| 14 | Thu, June 18 | Dimensionality Reduction and Penalized Regression | PCA and glmnet Lab |
| 15 | Fri, June 19 | Reproducible Research and Course Capstone | Capstone Lab & Presentations |

**Key packages:** `GEOquery`, `Biobase`, `DESeq2`, `edgeR`, `pheatmap`, `ComplexHeatmap`, `glmnet`, `factoextra`, `quarto`

---

## Software Requirements

All labs use R and RStudio. Please install the following before the course begins.

**Install R:** https://cran.r-project.org/

**Install RStudio:** https://posit.co/download/rstudio-desktop/

**Install core packages** by running the following in your R console:

```r
install.packages(c(
  "tidyverse", "rmarkdown", "quarto",
  "pROC", "survival", "survminer",
  "lme4", "caret", "rsample",
  "glmnet", "factoextra", "pheatmap"
))
```

**Install Bioconductor packages** (Week 3):

```r
if (!require("BiocManager", quietly = TRUE))
  install.packages("BiocManager")

BiocManager::install(c("DESeq2", "edgeR", "GEOquery", "Biobase", "ComplexHeatmap"))
```

If you run into any installation issues, please reach out before the course starts.

---

## About SC INBRE

This course is offered through the [South Carolina IDeA Networks of Biomedical Research Excellence (SC INBRE)](https://www.scinbre.org), supported by a grant from the National Institutes of Health National Institute of General Medical Sciences (P20GM103499). The course is free and open to SC INBRE participants, with priority given to SC INBRE-affiliated researchers.

**In-person location:**
USC Columbia, Discovery Building Computing Lab
915 Greene St., Suite 303B, Columbia, SC 29208
Paid parking: Innovista Parking Garage, 821 Park St., Columbia

---

## Contact

For questions about course content, please open a GitHub issue or contact Dr. McLain through the [Arnold School of Public Health faculty directory](https://sc.edu/study/colleges_schools/public_health/faculty-staff/mclain_alexander.php).

For registration and logistics questions, visit the [SC INBRE course page](https://www.scinbre.org/learning/bids-tutorials-and-workshops/2026-summer-workshop).
