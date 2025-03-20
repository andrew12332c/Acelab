# ACE Lab - Math Anxiety and Related Factors Analysis

## Overview
This repository contains the code and data for analyzing math anxiety and its relationship with various factors, including math self-efficacy, procrastination, and personal traits. The analysis uses survey data to assess how different factors contribute to math anxiety levels in students.

## Key Features
- **Survey Data Processing**: This project utilizes Likert scale survey responses to explore math anxiety and related factors.
- **Data Visualization**: The project generates box plots and Likert scale bar charts for visualizing the distribution of survey responses.
- **Statistical Analysis**: The analysis includes Kruskal-Wallis and pairwise Wilcoxon tests to examine significant differences across survey questions.
- **Data Wrangling**: The data is cleaned and transformed using R packages like `dplyr`, `tidyr`, and `ggplot2` for statistical analysis and visualization.

## Project Structure
```
/ace-lab
  ├── index.html              # Homepage of the project
  ├── data/                   # Folder containing the survey data file
      └── survey_data.csv     # The anonymized survey data used in analysis
  ├── R/                      # Folder containing R scripts for data processing
      ├── data_processing.R   # Data cleaning and transformation script
      ├── analysis.R          # Statistical analysis and visualization script
  └── README.md               # Project documentation
```

## Requirements
To run the analysis scripts in this project, you need the following packages in R:
- `tidyr`
- `ggplot2`
- `likert`
- `dplyr`
- `stringr`

You can install these packages using the following command in R:
```r
install.packages(c("tidyr", "ggplot2", "likert", "dplyr", "stringr"))
```

## Instructions

### 1. Data Loading
The survey data is loaded from a `.csv` file, which is stored in the `data` folder. The dataset contains responses to Likert scale questions on math anxiety, math self-efficacy, procrastination, and personal traits.

```r
df <- read.csv("data/survey_data.csv")
```

### 2. Data Processing
The data is processed using the `dplyr` and `tidyr` packages, including:
- Conversion of Likert scale responses into ordered factors.
- Transformation of data for visualization using `ggplot2`.

### 3. Data Visualization
Two types of plots are generated:
- **Box Plots**: To visualize the distribution of Likert scale responses.
- **Likert Bar Charts**: To show the distribution of responses for each question.

### 4. Statistical Analysis
- **Kruskal-Wallis Test**: For non-parametric comparison of response distributions across questions.
- **Pairwise Wilcoxon Test**: To identify significant differences between individual questions.

### 5. Output
The output of the analysis is saved as images (e.g., `likert_5_point.png`, `likert_7_point.png`) and displayed within the RStudio environment.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
For any questions, please feel free to open an issue or contact me directly via email.

---
