# Dataset Analysis Report: media.md

## Dataset Summary

**Shape:** (2652, 8)

**Columns:**

date, language, type, title, by, overall, quality, repeatability

## Insights and Analysis

### Key Statistics

Total rows: 2652, Total columns: 8

### Descriptive Statistics:
             date language   type              title                 by      overall      quality  repeatability
count        2553     2652   2652               2652               2390  2652.000000  2652.000000    2652.000000
unique       2055       11      8               2312               1528          NaN          NaN            NaN
top     21-May-06  English  movie  Kanda Naal Mudhal  Kiefer Sutherland          NaN          NaN            NaN
freq            8     1306   2211                  9                 48          NaN          NaN            NaN
mean          NaN      NaN    NaN                NaN                NaN     3.047511     3.209276       1.494721
std           NaN      NaN    NaN                NaN                NaN     0.762180     0.796743       0.598289
min           NaN      NaN    NaN                NaN                NaN     1.000000     1.000000       1.000000
25%           NaN      NaN    NaN                NaN                NaN     3.000000     3.000000       1.000000
50%           NaN      NaN    NaN                NaN                NaN     3.000000     3.000000       1.000000
75%           NaN      NaN    NaN                NaN                NaN     3.000000     4.000000       2.000000
max           NaN      NaN    NaN                NaN                NaN     5.000000     5.000000       3.000000

### Correlation Analysis:
                overall   quality  repeatability
overall        1.000000  0.825935       0.512600
quality        0.825935  1.000000       0.312127
repeatability  0.512600  0.312127       1.000000

### Missing Values:
date     99
by      262


## Description of Analysis

Sure! Here's a summary of the analysis of the dataset in straightforward language:

### Overview of the Dataset
- **Total Rows**: The dataset contains 2,652 entries (or records).
- **Total Columns**: There are 8 different types of information (or fields) in each entry.

### Descriptive Statistics
- **Date and Language**: There are 2,553 entries with dates and 2,652 with the language specified. The most common language is English, which appears 1,306 times.
- **Types of Content**: The dataset includes 8 different types of content, with "movie" being the most frequent type at 2,211 entries.
- **Titles**: There are 2,312 unique titles with "Kanda Naal Mudhal" being the most repeated title, occurring 9 times.
- **User Ratings**: Two fields provide numerical rating information:
  - **Overall Rating**: The average overall rating across entries is approximately 3.05 (on a scale of 1 to 5), with ratings ranging from a minimum of 1 to a maximum of 5.
  - **Quality Rating**: The average quality rating is about 3.21, with similar range limits.
  - **Repeatability Rating**: This rating has an average of about 1.49, with values ranging from 1 to a maximum of 3.

### Performance Metrics
- Median ratings show that most entries have a rating of 3 for both overall and quality, indicating that many ratings are average.
- The standard deviations for overall and quality ratings indicate that there is some variation in ratings; however, they are notably clustered around the average.

### Correlation Analysis
- There are relationships between the ratings:
  - **Overall and Quality Ratings**: High correlation (0.83) suggests that if a user's overall rating is high, the quality rating is likely to be high too.
  - **Overall and Repeatability Ratings**: There's a moderate correlation (0.51), meaning there's some connection but it's not very strong.
  - **Quality and Repeatability Ratings**: A low correlation (0.31) indicates these two ratings don't relate very closely to each other.

### Missing Values
- The dataset has some missing values:
  - **Dates**: 99 entries do not have a date.
  - **Creators (by)**: 262 entries are missing information about who created or performed the content.

### Overall Summary
This analysis gives insights into the dataset, highlighting that it consists mainly of movie entries with a focus on English content. Most ratings are around average, and there’s a general trend where high overall ratings tend to correlate with high quality ratings. However, there is a significant amount of missing data that could impact further analyses.

## Visualizations and Descriptions

### overall Distribution
![overall_distribution](outputs\graphs\overall_distribution.png)

The graph above shows the distribution of the 'overall' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 3.05, and the standard deviation is 0.76.

### quality Distribution
![quality_distribution](outputs\graphs\quality_distribution.png)

The graph above shows the distribution of the 'quality' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 3.21, and the standard deviation is 0.80.

### repeatability Distribution
![repeatability_distribution](outputs\graphs\repeatability_distribution.png)

The graph above shows the distribution of the 'repeatability' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 1.49, and the standard deviation is 0.60.

