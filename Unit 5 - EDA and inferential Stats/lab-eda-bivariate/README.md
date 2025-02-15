# Lab - EDA Bivariate Analysis: Diving into Amazon UK Product Insights Part II

## Objective:
Delve into the dynamics of product pricing on Amazon UK to uncover insights that can inform business strategies and decision-making.

## Dataset:
This lab utilizes the [Amazon UK product dataset](https://www.kaggle.com/datasets/asaniczka/uk-optimal-product-price-prediction/) which provides information on product categories, brands, prices, ratings, and more from Amazon UK. You'll need to download it to start working with it.

---

### Part 1: Analyzing Best-Seller Trends Across Product Categories

**Objective**: Understand the relationship between product categories and their best-seller status.

1. **Crosstab Analysis**:
    - Create a crosstab between the product `category` and the `isBestSeller` status.
    - Are there categories where being a best-seller is more prevalent?

2. **Statistical Tests**:
    - Conduct a Chi-square test to determine if the best-seller distribution is independent of the product category.
    - Compute Cramér's V to understand the strength of association between best-seller status and category.

3. **Visualizations**:
    - Visualize the relationship between product categories and the best-seller status using a stacked bar chart.

---

### Part 2: Exploring Product Prices and Ratings Across Categories and Brands

**Objective**: Investigate how different product categories influence product prices.

0. **Preliminary Step**: Remove outliers in product prices.

1. **Violin Plots**:
    - Use a violin plot to visualize the distribution of `price` across different product `categories`.

2. **Bar Charts**:
    - Create a bar chart comparing the average price of products for the top 10 product categories.

3. **Box Plots**:
    - Visualize the distribution of product `ratings` based on their `category` using side-by-side box plots.

---

### Part 3: Investigating the Interplay Between Product Prices and Ratings

**Objective**: Analyze how product ratings (`stars`) correlate with product prices.

1. **Correlation Coefficients**:
    - Calculate the correlation coefficient between `price` and `stars`.

2. **Visualizations**:
    - Use a scatter plot to visualize the relationship between product rating and price.
    - Use a correlation heatmap to visualize correlations between all numerical variables.
    - Examine if product prices typically follow a normal distribution using a QQ plot.

---

**Submission**: Submit a Jupyter Notebook which contains code and a business-centric report summarizing your findings.
