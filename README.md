# A/B Testing Marketing Promotions

This notebook analyzes A/B testing results for three marketing promotions at a fast food chain. It uses visualizations and t-tests to determine which promotion is most effective in increasing sales of a new menu item.

## Scenario

A fast food chain wants to add a new item to its menu and needs to decide between three marketing campaigns. To identify the most effective promotion, the new item is introduced at locations in randomly selected markets, with each location using a different promotion. Weekly sales data is collected for the first four weeks.

## Dataset

The dataset contains 548 entries with the following features:

- `MarketID`: An in-house tag for market types (not used in the analysis).
- `AgeOfStores`: Age of the store in years (1–28).
- `LocationID`: Unique identifier for store location.
- `Promotion`: One of three promotions tested (1, 2, 3).
- `SalesInThousands`: Sales amount for a specific location, promotion, and week.
- `MarketSize`: Size of the market (small, medium, or large).
- `Week`: One of four weeks when the promotions were run (1–4).

## Analysis

The notebook performs the following analysis:

* **Exploratory Data Analysis (EDA):** Uses visualizations (pie charts, bar charts) to explore the distribution of sales across promotions, market sizes, and store ages.
* **A/B Testing:** Conducts t-tests to compare the sales performance of different promotion groups (Promotion 1 vs. Promotion 2 and Promotion 1 vs. Promotion 3).
* **Statistical Significance:** Evaluates the t-values and p-values to determine if the differences in sales between promotion groups are statistically significant.

## Key Findings

* **Promotion Effectiveness:**  T-tests reveal that Promotion 1 significantly outperforms Promotion 2, but the difference between Promotion 1 and Promotion 3 is not statistically significant.
* **Store Age:** The analysis demonstrates that the store age distributions are similar across promotion groups, ensuring a fair comparison.

## Dependencies

This project requires the following Python libraries:

* pandas
* matplotlib
* scipy

You can install them using pip:

```bash
pip install pandas matplotlib scipy
```

## Usage

1. Clone the repository: `git clone https://github.com/your-username/ab-testing-promotions.git`
2. Install the dependencies (see above).
3. Open and run the Jupyter Notebook: `jupyter notebook ab-testing-promotions.ipynb`


## Contributing

Feel free to fork the repository and contribute by:

* Performing further analysis to understand the impact of `MarketSize` on promotion effectiveness.
* Conducting ANOVA tests to compare all three promotion groups simultaneously.
* Adding visualizations to illustrate the t-test results.
* Providing suggestions for further analysis.
