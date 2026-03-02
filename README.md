# Airbnb Price Determinants in European Cities

Authors: Shivani Aggarwal, Tina Yu, Anthony Leong, Brian Ni

## Project Overview

This project investigates the factors influencing Airbnb pricing across major European cities. By leveraging a comprehensive dataset of listings on the Airbnb platform, we analyze how social dynamics, geographic location, and host attributes impact the total listing price.

The analysis employs spatial econometric methods and regularized regression models to identify the most significant determinants of price.

### Methodology

To understand the dataset, we first conducted an exploratory data analysis to visualize price distributions and spatial trends.

To identify the most significant determinants of Airbnb prices, we performed feature selection and compared the performance of three predictive models: Stepwise AIC, LASSO, and Ridge Regression.

After evaluating each approach on a large validation set, we selected the machine learning model with the lowest RMSE score (Ridge Regression: 196.96). This indicates that the Ridge model provided the most accurate predictions and handled the high-dimensional dataset with the least amount of error compared to the other candidates.

## Setup & Installation

This project uses `renv` for dependency management. To recreate the environment:

1. Open R in the project root.
2. Run `install.packages("renv")` (if not already installed).
3. Run `renv::restore()`.

This will look at the `renv.lock` file and install the exact versions of the packages used during development.

## References

Barron, K., Kung, E., & Proserpio, D. (2019). *When Airbnb Listings in a City Increase, So Do Rent Prices.* Harvard Business Review. https://ci.carmel.ca.us/sites/main/files/file-attachments/harvard_business_article_and_study.pdf

Deboosere, R., Kerrigan, D. J., Wachsmuth, D., & El-Geneidy, A. (2019). *Location, location and professionalization: a multilevel hedonic analysis of Airbnb listing prices and revenue.* Regional Studies, Regional Science, 6(1), 143–156. https://doi.org/10.1080/21681376.2019.1592699

Gyódi, K., & Nawaro Ł. (2021). *Determinants of Airbnb prices in European cities: A spatial econometrics approach*. https://doi.org/10.1016/j.tourman.2021.104319