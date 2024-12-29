# Quantifying Effects of Solar Power Adoption on CO2 Emissions Reduction

A data-driven approach to estimate the immediate and time-lagged effects of an hourly increase in solar power generation on carbon dioxide (CO2) emissions reduction within the same geographic region and neighboring regions.

## Data

The datasets and more details about the data are available in [Dataverse](https://doi.org/10.7910/DVN/OKEATQ).

Download the files and store them in a folder `data` within the working directory.

## Description of the files

1.  `PreprocessingData.Rmd` contains the data preprocessing steps and stores the clean datasets for each region in separate .csv files within a folder called "data".
2.  `DistributedLagModelGeneration.Rmd` contains the script to generate the models aiding the estimations. It creates a folder called `tdlm_models` within the current working directory to store the generated models. Due to the complexity of the computations, executing this file may take several days.
3.  `Plot.Rmd` contains the script to generate the figures and tables. It creates a folder called `output` in the current working directory and stores all the results.

## Main Result

Combining the regional and interregional analyses, a substantial reduction of 633 million metric tons of CO2 emissions is found to be associated with a 15% increase in solar power generation across the US electricity sector over the next two decades.

![**Figure**: The estimated change in CO2 emissions (x-axis) in each region (colors) over the next two decades, associated with increased solar generation at every hour of the day within each region and also in the neighboring regions. Each horizontal bar corresponds to a specific percentage increase in solar generation (5%, 10%, 15%, and 20%). Within each horizontal bar, the colored segments represent the estimated CO2 reductions in different U.S. regions (such as California, Carolinas, Central, etc.). The black vertical line shows the target CO2 reduction value of 617 million metric tons.](output/total.png)
