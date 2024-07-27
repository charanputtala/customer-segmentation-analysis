# Sales Data Analysis with Google Colab and Tableau

## Project Overview

This project involves analyzing sales data, customer segmentation, and trends using both Google Colab and Tableau. The goal is to derive actionable insights through visualizations, covering top-selling items, revenue analysis, order frequency, user demographics, and more.

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Analysis and Insights](#analysis-and-insights)
  - [Top Selling Items](#top-selling-items)
  - [Revenue Analysis](#revenue-analysis)
  - [Order Frequency](#order-frequency)
  - [User Demographics](#user-demographics)
- [Tools Used](#tools-used)
- [How to Use](#how-to-use)
- [Contributing](#contributing)
- [License](#license)

## Data Sources

- `cleaned_items.csv`: Contains item details including item name, price, and quantity.
- `cleaned_user_details.csv`: Contains user information such as user ID, customer type, and registration dates.
- `cleaned_orders_list.csv`: Contains order details including order ID, user ID, order date, and payment information.

## Data Cleaning and Preparation

Data cleaning and preparation were performed in Google Colab using Python. The following steps were taken:

1. Loaded the data from CSV files.
2. Handled missing values and converted data types.
3. Saved the cleaned data as new CSV files for use in Tableau.

The cleaned data files are:

- `cleaned_items.csv`
- `cleaned_user_details.csv`
- `cleaned_orders_list.csv`

## Analysis and Insights

The analysis was conducted in Tableau, and the following insights were derived:

### Top Selling Items

- Identified the items with the highest sales volume.
- Determined the most frequently ordered items.

### Revenue Analysis

- Identified the items generating the most revenue.
- Calculated the average price of items sold.

### Order Frequency

- Analyzed the number of orders placed per day/week/month.
- Determined peak ordering times and days.

### User Demographics

- Analyzed the breakdown of B2C vs. B2B customers.
- Determined the number of new user registrations each month.

## Tools Used

- **Google Colab**: For data cleaning and preparation using Python.
- **Tableau**: For data visualization and deriving insights.

## How to Use

1. **Data Cleaning and Preparation**:
   - Open the `data_cleaning.ipynb` notebook in Google Colab.
   - Run the notebook to load, clean, and save the data.

2. **Visualization in Tableau**:
   - Import the cleaned CSV files into Tableau.
   - Create relationships between the tables:
     - Items and Orders: `order_id_fk` in `cleaned_items.csv` = `order_id` in `cleaned_orders_list.csv`.
     - Orders and Users: `user_id` in `cleaned_orders_list.csv` = `id` in `cleaned_user_details.csv`.
   - Create visualizations for different insights as outlined in the [Analysis and Insights](#analysis-and-insights) section.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue to discuss changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
