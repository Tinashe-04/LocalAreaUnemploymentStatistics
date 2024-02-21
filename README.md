# LocalAreaUnemploymentStatistics
A repository with code for exploratory data analysis of unemployment statistics in California

01/16/2024

- Found out that the status of the data collection is split into 3: Preliminary, prelim, and final
- Found out that all data points up to June 2023 are 'final' statistics
- To make it easier, we will assume that preliminary means these data points are not conclusive and therefore cannot be accurate for use in a statistical analysis
- Filtered out the data entries that are preliminary at the same time as seasonally adjusted alteration is made
- Computed median of unemployment rates by year
- Added percentage column for unemployment rates
- To do next: check if June 2023 is the latest date in the dataset (helps with working on time-series data too)
- To do next: Revise all mean plots
- To do next: Answer the questions added to the notebook

01/30/2024

- Added percentage change plot to the labor force data
- revised all mean plots and changed them to median
- I had asked 7 questions of the data. As of this day I have answered 2 questions using plots and code.
- Thinking of adding a couple more questions, such as is there a correlation between labor force size and unemployment rates?
- Changed 'date' column to datetime type and could be explored further
- found out that unemployment rates are most frequent between 5% and 10% which can be a useful metric for unemployment observers, economists
- found out that 2020 had the largest percentage change in size of labor force (think COVID)
- TODO: check if June 2023 is the latest date in the dataset (helps with working on time-series data too)
- TODO: add line at y=0 for percentage changes
- TODO: Provide summary statements for the boxplots
- TODO: Answer the questions added to the notebook

02/21/2024

- I used sklearn's LinearRegression class to come up with a regression equation that estimates the unemployment rate based on the size of the labor force
- I found out that for every additional person who is added to the labor force, the unemployment rate decreases by 1.08e-09.
- In other words, solely based on the size of the labor force, it will take just over 9,000,000 people to be added to the labor force for the unemployment rate to decrease by 0.01 or by 1%.
- There is more to come.
- TODO: check if June 2023 is the latest date in the dataset (helps with working on time-series data too)
- TODO: add line at y=0 for percentage changes
- TODO: Provide summary statements for the boxplots
- TODO: Answer the questions added to the notebook

Additionally, I outlined the stakeholders interested in LAUS data directly from the BLS website (https://www.bls.gov/lau/lauov.htm) to get a better sense of who would be interested in the insights gathered from the LAUS data. They are detailed as follows.

A wide variety of customers use these estimates:

- Federal programs use the data for allocations to states and areas, as well as eligibility determinations for assistance.
- State and local governments use the estimates for planning and budgetary purposes and to determine the need for local employment and training services.
- Private industry, researchers, the media, and other individuals use the data to assess localized labor market developments and make comparisons across areas.


