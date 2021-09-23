# sg-income-dist
This project attempts to build a parametric distribution of monthly household income from work in Singapore. The estimated distribution can be used to calculate various statistics of interest, e.g., percentiles.

The main challenge is that raw data of individual household income are not available for privacy reason. Only aggregate data such as the population mean, median,
and average income per decile are published by the [Singapore Department of Statistics](https://www.singstat.gov.sg).  

# Methodology
1. Aggregate data on monthly household income from work ([1], [2]) are collected and processed.
2. A parametric family of distributions is selected. The following three families are/will be considered following the recommendations by [3]:
    * Weibull
    * Dagum (TODO)
    * Generalized beta of the second kind (TODO)
3. Distribution parameters are optimized by minimizing the discrepancy between the aggregate data and the model prediction.

# References
1. Standard Chartered Bank, 2020. [Singapore average monthly household income from work in 2019](https://av.sc.com/sg/content/images/StanChart_Ave-Income_MINI-2_850.png).
1. Department of Statistics Singapore, 2021. [Key Household Income Trends, 2020](https://www.singstat.gov.sg/-/media/files/visualising_data/infographics/households/key-household-income-trends-2020.pdf).
1. Ripsy Bandourian, Robert Turley, and James McDonald, 2002.  "[A Comparison of Parametric Models of Income Distribution across Countries and over Time](http://www.lisdatacenter.org/wps/liswps/305.pdf)".

[1]: https://av.sc.com/sg/content/images/StanChart_Ave-Income_MINI-2_850.png 
[2]: https://www.singstat.gov.sg/-/media/files/visualising_data/infographics/households/key-household-income-trends-2020.pdf 
[3]: http://www.lisdatacenter.org/wps/liswps/305.pdf
