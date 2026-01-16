# PySpark E-commerce Data Analysis
[![Ask DeepWiki](https://devin.ai/assets/askdeepwiki.png)](https://deepwiki.com/Ilia20062/work)

This repository contains a Jupyter notebook demonstrating fundamental data analysis operations using PySpark. It processes a sample e-commerce event dataset to extract meaningful insights.

## Dataset

The analysis is performed on a small, self-contained dataset representing user interactions on an e-commerce platform. The data is embedded directly within the notebook as a multi-line string and includes the following fields:

*   `event_id`: Unique identifier for the event.
*   `user_id`: Identifier for the user.
*   `event_ts`: Timestamp of the event.
*   `event_type`: Type of event (e.g., `view`, `add_to_cart`, `purchase`, `refund`).
*   `product_category`: Category of the product involved.
*   `price`: Price of the product (negative for refunds).
*   `device`: Device used by the user.
*   `country`: User's country.

## Analysis Examples

The `MyFirstNotebook.ipynb` notebook demonstrates several common data analysis tasks:

1.  **Data Ingestion and Preparation**: Reading raw text data into a Spark DataFrame and casting columns to their appropriate data types (Integer, Timestamp, Double).
2.  **Event Aggregation**: Counting the total number of events for each `event_type`.
3.  **Purchase Analytics**: Identifying the top 3 countries with the highest number of purchases.
4.  **Revenue Calculation**: Calculating the total net revenue by summing the prices for `purchase` and `refund` events.
5.  **User Behavior Analysis**: Identifying users who have viewed products more than once but have not completed a purchase.

## Getting Started

### Prerequisites

*   Python
*   A running PySpark installation (which requires Java and Apache Spark).
*   A Jupyter Notebook environment or a compatible IDE (e.g., VS Code with the Jupyter extension).

### Execution

1.  Clone this repository to your local machine.
2.  Open the `MyFirstNotebook.ipynb` file in your Jupyter environment.
3.  Execute the cells sequentially to initialize the Spark session, create the DataFrame, and perform the analyses.
