# dam-final-project.2025
Aarhus University final project in Digital archives and Methods

# Tracing Political Priorities Through Text Mining: A Comparative Study of Danish Party Programmes (1979–1981)

## Authors
Josefine Dresler & Lars Hesel

## Overview

This project uses text mining techniques to analyze and compare political themes in Danish party programmes from **Socialdemokratiet** and **Det Konservative Folkeparti** during the election years of **1979–1981**. By identifying frequently used bigrams and mapping them to key policy areas, the project visualizes how rhetorical focus shifted over time.

This work is part of the Digital Archives & Methods course at Aarhus University.

## Repository Contents
data_DAMprojekt/tidy_data/
- konservative_1980.txt
- konservative_1981.txt
- socialdemokratiet_1979.txt
- socialdemokratiet_1981.txt

output/
- konservative_temaoversigt_1980_1981.pdf
- socialdemokratiet_temaoversigt_1979_1981.pdf

final_project.Rmd # Main analysis script
README.md

## Features
- Bigram tokenization using the `tidytext` package
- Regular expression–based thematic classification
- Comparative bar chart visualizations of theme frequency per year and party
- Exported high-quality visualizations for reporting

## Installation & Reproduction

To reproduce the analysis:

1. Clone this repository:
   ```bash
   git clone https://github.com/jdresler/dam-final-project.2025.git
2. Open final_project.Rmd in RStudio.
3. Make sure the following R packages are installed:
   install.packages(c("tidyverse", "tidytext", "stringr", "readr"))
5. Run all chunks in final_project.Rmd.
   This will:
   Read the .txt party programmes
   Tokenize text into bigrams
   Map each bigram to a political theme
   Count and plot theme frequency per year
   Export final figures as PDF

## Requirements
- R 4.4.0
- RStudio 2024.04.0
- tidyverse
- tidytext
- stringr
- readr

## Acknowledgements 
- Inspired by approaches outlined in:
  Tahmasebi & Hengchen (2019), The Strengths and Pitfalls of Large-Scale Text Mining for Literary Studies
- Wickham (2014), Tidy Data

## Files
- `socialdemokratiet_1979.txt` – OCR-processed party programme
- `socialdemokratiet_1981.txt`
- `konservative_1980.txt`
- `konservative_1981.txt`
- `analysis.Rmd` – Code for running the analysis
- `socialdemokratiet_temaoversigt_1979_1981.pdf` – Theme frequency chart for Socialdemokratiet
- `konservative_temaoversigt_1980_1981.pdf` – Theme frequency chart for Konservative

## How to Run
1. Open `analysis.Rmd` in RStudio.
2. Run all code chunks or knit to generate visualizations.
3. Output is saved as PDF files.

This project is for academic purposes and part of a university course. All included data and visualizations are derived from publicly available party programme materials via The Royal Danish Library.
