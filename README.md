# A/B testing analysis

Using data from an e-commerce website, this analysis looks at whether a new landing page was effective at getting more visitors to "convert", i.e. decide to pay for a company's product.

## Methods of Analysis

1. Probability
2. Bootstrapping a sample for A/B testing
3. Logistic regression

## Data

First 5 rows of data looks like this:
|    |   user_id | timestamp                  | group     | landing_page   |   converted |
|---:|----------:|:---------------------------|:----------|:---------------|------------:|
|  0 |    851104 | 2017-01-21 22:11:48.556739 | control   | old_page       |           0 |
|  1 |    804228 | 2017-01-12 08:01:45.159739 | control   | old_page       |           0 |
|  2 |    661590 | 2017-01-11 16:55:06.154213 | treatment | new_page       |           0 |
|  3 |    853541 | 2017-01-08 18:28:03.143765 | treatment | new_page       |           0 |
|  4 |    864975 | 2017-01-21 01:52:26.210827 | control   | old_page       |           1 |
