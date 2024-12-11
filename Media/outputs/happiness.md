# Dataset Analysis Report: happiness.md

## Dataset Summary

**Shape:** (2363, 11)

**Columns:**

Country name, year, Life Ladder, Log GDP per capita, Social support, Healthy life expectancy at birth, Freedom to make life choices, Generosity, Perceptions of corruption, Positive affect, Negative affect

## Insights and Analysis

### Key Statistics

Total rows: 2363, Total columns: 11

### Descriptive Statistics:
       Country name         year  Life Ladder  Log GDP per capita  Social support  Healthy life expectancy at birth  Freedom to make life choices   Generosity  Perceptions of corruption  Positive affect  Negative affect
count          2363  2363.000000  2363.000000         2335.000000     2350.000000                       2300.000000                   2327.000000  2282.000000                2238.000000      2339.000000      2347.000000
unique          165          NaN          NaN                 NaN             NaN                               NaN                           NaN          NaN                        NaN              NaN              NaN
top         Lebanon          NaN          NaN                 NaN             NaN                               NaN                           NaN          NaN                        NaN              NaN              NaN
freq             18          NaN          NaN                 NaN             NaN                               NaN                           NaN          NaN                        NaN              NaN              NaN
mean            NaN  2014.763860     5.483566            9.399671        0.809369                         63.401828                      0.750282     0.000098                   0.743971         0.651882         0.273151
std             NaN     5.059436     1.125522            1.152069        0.121212                          6.842644                      0.139357     0.161388                   0.184865         0.106240         0.087131
min             NaN  2005.000000     1.281000            5.527000        0.228000                          6.720000                      0.228000    -0.340000                   0.035000         0.179000         0.083000
25%             NaN  2011.000000     4.647000            8.506500        0.744000                         59.195000                      0.661000    -0.112000                   0.687000         0.572000         0.209000
50%             NaN  2015.000000     5.449000            9.503000        0.834500                         65.100000                      0.771000    -0.022000                   0.798500         0.663000         0.262000
75%             NaN  2019.000000     6.323500           10.392500        0.904000                         68.552500                      0.862000     0.093750                   0.867750         0.737000         0.326000
max             NaN  2023.000000     8.019000           11.676000        0.987000                         74.600000                      0.985000     0.700000                   0.983000         0.884000         0.705000

### Correlation Analysis:
                                      year  Life Ladder  Log GDP per capita  Social support  Healthy life expectancy at birth  Freedom to make life choices  Generosity  Perceptions of corruption  Positive affect  Negative affect
year                              1.000000     0.046846            0.080104       -0.043074                          0.168026                      0.232974    0.030864                  -0.082136         0.013052         0.207642
Life Ladder                       0.046846     1.000000            0.783556        0.722738                          0.714927                      0.538210    0.177398                  -0.430485         0.515283        -0.352412
Log GDP per capita                0.080104     0.783556            1.000000        0.685329                          0.819326                      0.364816   -0.000766                  -0.353893         0.230868        -0.260689
Social support                   -0.043074     0.722738            0.685329        1.000000                          0.597787                      0.404131    0.065240                  -0.221410         0.424524        -0.454878
Healthy life expectancy at birth  0.168026     0.714927            0.819326        0.597787                          1.000000                      0.375745    0.015168                  -0.303130         0.217982        -0.150330
Freedom to make life choices      0.232974     0.538210            0.364816        0.404131                          0.375745                      1.000000    0.321396                  -0.466023         0.578398        -0.278959
Generosity                        0.030864     0.177398           -0.000766        0.065240                          0.015168                      0.321396    1.000000                  -0.270004         0.300608        -0.071975
Perceptions of corruption        -0.082136    -0.430485           -0.353893       -0.221410                         -0.303130                     -0.466023   -0.270004                   1.000000        -0.274208         0.265555
Positive affect                   0.013052     0.515283            0.230868        0.424524                          0.217982                      0.578398    0.300608                  -0.274208         1.000000        -0.334451
Negative affect                   0.207642    -0.352412           -0.260689       -0.454878                         -0.150330                     -0.278959   -0.071975                   0.265555        -0.334451         1.000000

### Missing Values:
Log GDP per capita                   28
Social support                       13
Healthy life expectancy at birth     63
Freedom to make life choices         36
Generosity                           81
Perceptions of corruption           125
Positive affect                      24
Negative affect                      16


## Description of Analysis

Here’s a simplified breakdown of the analysis you provided regarding the dataset:

### Overview of the Dataset
- The dataset consists of **2363 rows** (each representing a data entry) and **11 columns** (representing different variables).
- The data focuses on various aspects of well-being in different countries over time.

### Descriptive Statistics
- **Country Names**: There are **165 unique country names** in the dataset, with Lebanon appearing **18 times**, which is the most frequent.
- **Years**: Data covers a time span with years ranging from **2005 to 2023**.
- **Life Ladder**: This is a measure of well-being. The average score is approximately **5.48**, with scores ranging from **1.28 to 8.02**.
- **Log GDP per capita**: This represents economic performance, with an average of about **9.40** and a range from **5.53 to 11.68**.
- **Social Support**: Measures how individuals perceive support from their communities. The average score is **0.81**.
- **Healthy Life Expectancy**: On average, people can expect to live healthily for about **63.4 years**, with a range from **6.72** to **74.6 years**.
- **Freedom to Make Life Choices**: The average freedom score is about **0.75**.
- **Generosity**: Measures how generous people are, averaging **0.0001** (very close to zero) with scores ranging from **-0.34 to 0.70**.
- **Perceptions of Corruption**: This has an average score of about **0.74**, indicating a moderate perception of corruption among individuals.
- **Positive Affect**: Average is **0.65**, which suggests a generally positive emotional state.
- **Negative Affect**: Average is **0.27**, suggesting lower levels of negative emotions.

### Correlation Analysis
This section examines the relationships between different variables:
- **Year and Life Ladder**: There's a slight positive correlation (**0.05**), meaning as time goes on, life satisfaction might slightly increase.
- **Life Ladder and Log GDP per capita**: A strong positive correlation (**0.78**) indicates that higher GDP is associated with higher life satisfaction.
- **Social Support and Happiness**: Similarly, a strong positive relationship (**0.72**) exists here, showing that better social support correlates with greater happiness.
- **Freedom to Make Life Choices** also shows a positive correlation (**0.54**) with life satisfaction.
- Interestingly, higher perceptions of corruption tend to be negatively correlated with life satisfaction (**-0.43**), indicating that the more people perceive corruption in their country, the less satisfied they are with life.
  
### Missing Values
Some data points are missing in the following categories:
- **Log GDP per capita**: 28 entries are missing.
- **Social support**: 13 entries are missing.
- **Healthy life expectancy at birth**: 63 entries are missing.
- **Freedom to make life choices**: 36 entries are missing.
- **Generosity**: 81 entries are missing.
- **Perceptions of corruption**: 125 entries are missing.
- **Positive affect**: 24 entries are missing.
- **Negative affect**: 16 entries are missing.

### Conclusion
Overall, the dataset provides insights into how various factors like economic performance, social support, and perceptions of corruption relate to individual well-being across different countries and years. There are some missing entries that may affect the completeness of the analysis, but the overall statistics and correlations give a clear picture of trends in well-being over time.

## Visualizations and Descriptions

### year Distribution
![year_distribution](outputs\graphs\year_distribution.png)

The graph above shows the distribution of the 'year' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 2014.76, and the standard deviation is 5.06.

### Life Ladder Distribution
![Life Ladder_distribution](outputs\graphs\Life Ladder_distribution.png)

The graph above shows the distribution of the 'Life Ladder' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 5.48, and the standard deviation is 1.13.

### Log GDP per capita Distribution
![Log GDP per capita_distribution](outputs\graphs\Log GDP per capita_distribution.png)

The graph above shows the distribution of the 'Log GDP per capita' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 9.40, and the standard deviation is 1.15.

### Social support Distribution
![Social support_distribution](outputs\graphs\Social support_distribution.png)

The graph above shows the distribution of the 'Social support' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 0.81, and the standard deviation is 0.12.

### Healthy life expectancy at birth Distribution
![Healthy life expectancy at birth_distribution](outputs\graphs\Healthy life expectancy at birth_distribution.png)

The graph above shows the distribution of the 'Healthy life expectancy at birth' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 63.40, and the standard deviation is 6.84.

### Freedom to make life choices Distribution
![Freedom to make life choices_distribution](outputs\graphs\Freedom to make life choices_distribution.png)

The graph above shows the distribution of the 'Freedom to make life choices' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 0.75, and the standard deviation is 0.14.

### Generosity Distribution
![Generosity_distribution](outputs\graphs\Generosity_distribution.png)

The graph above shows the distribution of the 'Generosity' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 0.00, and the standard deviation is 0.16.

### Perceptions of corruption Distribution
![Perceptions of corruption_distribution](outputs\graphs\Perceptions of corruption_distribution.png)

The graph above shows the distribution of the 'Perceptions of corruption' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 0.74, and the standard deviation is 0.18.

### Positive affect Distribution
![Positive affect_distribution](outputs\graphs\Positive affect_distribution.png)

The graph above shows the distribution of the 'Positive affect' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 0.65, and the standard deviation is 0.11.

### Negative affect Distribution
![Negative affect_distribution](outputs\graphs\Negative affect_distribution.png)

The graph above shows the distribution of the 'Negative affect' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 0.27, and the standard deviation is 0.09.

