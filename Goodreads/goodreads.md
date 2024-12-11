# Dataset Analysis Report: goodreads.md

## Dataset Summary

**Shape:** (10000, 23)

**Columns:**

book_id, goodreads_book_id, best_book_id, work_id, books_count, isbn, isbn13, authors, original_publication_year, original_title, title, language_code, average_rating, ratings_count, work_ratings_count, work_text_reviews_count, ratings_1, ratings_2, ratings_3, ratings_4, ratings_5, image_url, small_image_url

## Insights and Analysis

### Key Statistics

Total rows: 10000, Total columns: 23

### Descriptive Statistics:
            book_id  goodreads_book_id  best_book_id       work_id   books_count       isbn        isbn13       authors  original_publication_year original_title           title language_code  average_rating  ratings_count  work_ratings_count  work_text_reviews_count      ratings_1      ratings_2      ratings_3     ratings_4     ratings_5                                                                                 image_url                                                                         small_image_url
count   10000.00000       1.000000e+04  1.000000e+04  1.000000e+04  10000.000000       9300  9.415000e+03         10000                9979.000000           9415           10000          8916    10000.000000   1.000000e+04        1.000000e+04             10000.000000   10000.000000   10000.000000   10000.000000  1.000000e+04  1.000000e+04                                                                                     10000                                                                                   10000
unique          NaN                NaN           NaN           NaN           NaN       9300           NaN          4664                        NaN           9274            9964            25             NaN            NaN                 NaN                      NaN            NaN            NaN            NaN           NaN           NaN                                                                                      6669                                                                                    6669
top             NaN                NaN           NaN           NaN           NaN  439023483           NaN  Stephen King                        NaN                 Selected Poems           eng             NaN            NaN                 NaN                      NaN            NaN            NaN            NaN           NaN           NaN  https://s.gr-assets.com/assets/nophoto/book/111x148-bcc042a9c91a29c1d680899eff700a03.png  https://s.gr-assets.com/assets/nophoto/book/50x75-a91bf249278a81aabab721ef782c4a74.png
freq            NaN                NaN           NaN           NaN           NaN          1           NaN            60                        NaN              5               4          6341             NaN            NaN                 NaN                      NaN            NaN            NaN            NaN           NaN           NaN                                                                                      3332                                                                                    3332
mean     5000.50000       5.264697e+06  5.471214e+06  8.646183e+06     75.712700        NaN  9.755044e+12           NaN                1981.987674            NaN             NaN           NaN        4.002191   5.400124e+04        5.968732e+04              2919.955300    1345.040600    3110.885000   11475.893800  1.996570e+04  2.378981e+04                                                                                       NaN                                                                                     NaN
std      2886.89568       7.575462e+06  7.827330e+06  1.175106e+07    170.470728        NaN  4.428619e+11           NaN                 152.576665            NaN             NaN           NaN        0.254427   1.573700e+05        1.678038e+05              6124.378132    6635.626263    9717.123578   28546.449183  5.144736e+04  7.976889e+04                                                                                       NaN                                                                                     NaN
min         1.00000       1.000000e+00  1.000000e+00  8.700000e+01      1.000000        NaN  1.951703e+08           NaN               -1750.000000            NaN             NaN           NaN        2.470000   2.716000e+03        5.510000e+03                 3.000000      11.000000      30.000000     323.000000  7.500000e+02  7.540000e+02                                                                                       NaN                                                                                     NaN
25%      2500.75000       4.627575e+04  4.791175e+04  1.008841e+06     23.000000        NaN  9.780316e+12           NaN                1990.000000            NaN             NaN           NaN        3.850000   1.356875e+04        1.543875e+04               694.000000     196.000000     656.000000    3112.000000  5.405750e+03  5.334000e+03                                                                                       NaN                                                                                     NaN
50%      5000.50000       3.949655e+05  4.251235e+05  2.719524e+06     40.000000        NaN  9.780452e+12           NaN                2004.000000            NaN             NaN           NaN        4.020000   2.115550e+04        2.383250e+04              1402.000000     391.000000    1163.000000    4894.000000  8.269500e+03  8.836000e+03                                                                                       NaN                                                                                     NaN
75%      7500.25000       9.382225e+06  9.636112e+06  1.451775e+07     67.000000        NaN  9.780831e+12           NaN                2011.000000            NaN             NaN           NaN        4.180000   4.105350e+04        4.591500e+04              2744.250000     885.000000    2353.250000    9287.000000  1.602350e+04  1.730450e+04                                                                                       NaN                                                                                     NaN
max     10000.00000       3.328864e+07  3.553423e+07  5.639960e+07   3455.000000        NaN  9.790008e+12           NaN                2017.000000            NaN             NaN           NaN        4.820000   4.780653e+06        4.942365e+06            155254.000000  456191.000000  436802.000000  793319.000000  1.481305e+06  3.011543e+06                                                                                       NaN                                                                                     NaN

### Correlation Analysis:
                            book_id  goodreads_book_id  best_book_id   work_id  books_count    isbn13  original_publication_year  average_rating  ratings_count  work_ratings_count  work_text_reviews_count  ratings_1  ratings_2  ratings_3  ratings_4  ratings_5
book_id                    1.000000           0.115154      0.104516  0.113861    -0.263841 -0.011291                   0.049875       -0.040880      -0.373178           -0.382656                -0.419292  -0.239401  -0.345764  -0.413279  -0.407079  -0.332486
goodreads_book_id          0.115154           1.000000      0.966620  0.929356    -0.164578 -0.048246                   0.133790       -0.024848      -0.073023           -0.063760                 0.118845  -0.038375  -0.056571  -0.075634  -0.063310  -0.056145
best_book_id               0.104516           0.966620      1.000000  0.899258    -0.159240 -0.047253                   0.131442       -0.021187      -0.069182           -0.055835                 0.125893  -0.033894  -0.049284  -0.067014  -0.054462  -0.049524
work_id                    0.113861           0.929356      0.899258  1.000000    -0.109436 -0.039320                   0.107972       -0.017555      -0.062720           -0.054712                 0.096985  -0.034590  -0.051367  -0.066746  -0.054775  -0.046745
books_count               -0.263841          -0.164578     -0.159240 -0.109436     1.000000  0.017865                  -0.321753       -0.069888       0.324235            0.333664                 0.198698   0.225763   0.334923   0.383699   0.349564   0.279559
isbn13                    -0.011291          -0.048246     -0.047253 -0.039320     0.017865  1.000000                  -0.004612       -0.025667       0.008904            0.009166                 0.009553   0.006054   0.010345   0.012142   0.010161   0.006622
original_publication_year  0.049875           0.133790      0.131442  0.107972    -0.321753 -0.004612                   1.000000        0.015608      -0.024415           -0.025448                 0.027784  -0.019635  -0.038472  -0.042459  -0.025785  -0.015388
average_rating            -0.040880          -0.024848     -0.021187 -0.017555    -0.069888 -0.025667                   0.015608        1.000000       0.044990            0.045042                 0.007481  -0.077997  -0.115875  -0.065237   0.036108   0.115412
ratings_count             -0.373178          -0.073023     -0.069182 -0.062720     0.324235  0.008904                  -0.024415        0.044990       1.000000            0.995068                 0.779635   0.723144   0.845949   0.935193   0.978869   0.964046
work_ratings_count        -0.382656          -0.063760     -0.055835 -0.054712     0.333664  0.009166                  -0.025448        0.045042       0.995068            1.000000                 0.807009   0.718718   0.848581   0.941182   0.987764   0.966587
work_text_reviews_count   -0.419292           0.118845      0.125893  0.096985     0.198698  0.009553                   0.027784        0.007481       0.779635            0.807009                 1.000000   0.572007   0.696880   0.762214   0.817826   0.764940
ratings_1                 -0.239401          -0.038375     -0.033894 -0.034590     0.225763  0.006054                  -0.019635       -0.077997       0.723144            0.718718                 0.572007   1.000000   0.926140   0.795364   0.672986   0.597231
ratings_2                 -0.345764          -0.056571     -0.049284 -0.051367     0.334923  0.010345                  -0.038472       -0.115875       0.845949            0.848581                 0.696880   0.926140   1.000000   0.949596   0.838298   0.705747
ratings_3                 -0.413279          -0.075634     -0.067014 -0.066746     0.383699  0.012142                  -0.042459       -0.065237       0.935193            0.941182                 0.762214   0.795364   0.949596   1.000000   0.952998   0.825550
ratings_4                 -0.407079          -0.063310     -0.054462 -0.054775     0.349564  0.010161                  -0.025785        0.036108       0.978869            0.987764                 0.817826   0.672986   0.838298   0.952998   1.000000   0.933785
ratings_5                 -0.332486          -0.056145     -0.049524 -0.046745     0.279559  0.006622                  -0.015388        0.115412       0.964046            0.966587                 0.764940   0.597231   0.705747   0.825550   0.933785   1.000000

### Missing Values:
isbn                          700
isbn13                        585
original_publication_year      21
original_title                585
language_code                1084


## Description of Analysis

Sure! Lets break down the analysis of the dataset into simpler terms.

### Overview of the Dataset
- The dataset contains **10,000 rows** and **23 columns**. Each row represents a different book, while the columns provide various details about those books.

### Key Information About the Books
- **Descriptive Statistics**: This section gives us summary information about the fields in the dataset.
  - **book_id**: A unique identifier for each book.
  - **goodreads_book_id** and **best_book_id**: Identifiers that are used on certain platforms.
  - **authors**: The name of the author(s) of the book.
  - **original_publication_year**: Year when the book was first published.
  - **title**: The title of the book.
  - **average_rating**: The average rating given to the book by readers on a scale (usually 1 to 5).
  - **ratings_count**: The total number of ratings the book has received.
  - **work_ratings_count**: Total ratings for the books specific edition or work.
  - **ratings_1 to ratings_5**: The number of readers who rated the book with 1, 2, 3, 4, and 5 stars.

#### Summary Statistics:
- The **average rating** across books is about **4.00**, which indicates that most books are generally well-liked.
- The **ratings count** can be significantly high for some books, showing they are more popular or widely read.
- The **original publication year** for most books ranges from around **1981 to 2017**.

### Observations on Unique Values
- There are **4,664 unique titles** in the dataset, meaning many books are represented multiple times (for instance, different editions).
- **Top Author**: The most frequent author in the dataset is **Stephen King**, with **60 entries**.

### Relationships Between Variables (Correlation Analysis)
- The correlation analysis shows how different features relate to each other.
  - A lower **books_count** (how many books an author has) is related to higher **ratings_count** and **work_ratings_count**. This might suggest that authors with fewer books but quality content tend to get more attention.
  - **Ratings_count** and **work_ratings_count** are highly correlated (0.995), meaning books that get many ratings likely have a lot of ratings on their specific editions too.
  - Conversely, average ratings dont show strong correlations with **ratings_count**, implying that more ratings do not necessarily mean a higher average score.

### Missing Values
- The dataset has some missing values:
  - **isbn**: Missing for **700** books.
  - **isbn13**: Missing for **585** books.
  - **original_publication_year**: Missing for **21** books.
  - **original_title**: Missing for **585** books.
  - **language_code**: Missing for **1,084** books.

This suggests that there are several books for which complete information isnt available. 

### Conclusion
In simple terms, this dataset is a rich compilation of book-related information that includes details about the books, authors, publication years, ratings, and their relationships. The findings indicate that most books are well-rated, especially those with unique authorship and good number of ratings. However, there are also missing pieces in some of the data that might need addressing for further analysis.

## Visualizations and Descriptions

### book_id Distribution
![book_id_distribution](outputs/graphs/book_id_distribution.png)

The graph above shows the distribution of the 'book_id' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 5000.50, and the standard deviation is 2886.90.

### goodreads_book_id Distribution
![goodreads_book_id_distribution](outputs/graphs/goodreads_book_id_distribution.png)

The graph above shows the distribution of the 'goodreads_book_id' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 5264696.51, and the standard deviation is 7575461.86.

### best_book_id Distribution
![best_book_id_distribution](outputs/graphs/best_book_id_distribution.png)

The graph above shows the distribution of the 'best_book_id' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 5471213.58, and the standard deviation is 7827329.89.

### work_id Distribution
![work_id_distribution](outputs/graphs/work_id_distribution.png)

The graph above shows the distribution of the 'work_id' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 8646183.42, and the standard deviation is 11751060.82.

### books_count Distribution
![books_count_distribution](outputs/graphs/books_count_distribution.png)

The graph above shows the distribution of the 'books_count' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 75.71, and the standard deviation is 170.47.

### isbn13 Distribution
![isbn13_distribution](outputs/graphs/isbn13_distribution.png)

The graph above shows the distribution of the 'isbn13' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 9755044298883.46, and the standard deviation is 442861920665.57.

### original_publication_year Distribution
![original_publication_year_distribution](outputs/graphs/original_publication_year_distribution.png)

The graph above shows the distribution of the 'original_publication_year' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 1981.99, and the standard deviation is 152.58.

### average_rating Distribution
![average_rating_distribution](outputs/graphs/average_rating_distribution.png)

The graph above shows the distribution of the 'average_rating' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 4.00, and the standard deviation is 0.25.

### ratings_count Distribution
![ratings_count_distribution](outputs/graphs/ratings_count_distribution.png)

The graph above shows the distribution of the 'ratings_count' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 54001.24, and the standard deviation is 157369.96.

### work_ratings_count Distribution
![work_ratings_count_distribution](outputs/graphs/work_ratings_count_distribution.png)

The graph above shows the distribution of the 'work_ratings_count' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 59687.32, and the standard deviation is 167803.79.

### work_text_reviews_count Distribution
![work_text_reviews_count_distribution](outputs/graphs/work_text_reviews_count_distribution.png)

The graph above shows the distribution of the 'work_text_reviews_count' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 2919.96, and the standard deviation is 6124.38.

### ratings_1 Distribution
![ratings_1_distribution](outputs/graphs/ratings_1_distribution.png)

The graph above shows the distribution of the 'ratings_1' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 1345.04, and the standard deviation is 6635.63.

### ratings_2 Distribution
![ratings_2_distribution](outputs/graphs/ratings_2_distribution.png)

The graph above shows the distribution of the 'ratings_2' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 3110.89, and the standard deviation is 9717.12.

### ratings_3 Distribution
![ratings_3_distribution](outputs/graphs/ratings_3_distribution.png)

The graph above shows the distribution of the 'ratings_3' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 11475.89, and the standard deviation is 28546.45.

### ratings_4 Distribution
![ratings_4_distribution](outputs/graphs/ratings_4_distribution.png)

The graph above shows the distribution of the 'ratings_4' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 19965.70, and the standard deviation is 51447.36.

### ratings_5 Distribution
![ratings_5_distribution](outputs\graphs\ratings_5_distribution.png)

The graph above shows the distribution of the 'ratings_5' column. It visualizes the frequency distribution of the values. Look for the central tendency, spread, and any possible skewness in the distribution. From the descriptive statistics, the mean of this column is 23789.81, and the standard deviation is 79768.89.

