# Fake Data Generator

The `Fake Data Generator` is a tool designed to create realistic simulation data. The data is generated in three stages, covering customers, products, and sales, with seasonality considerations. Currently, it is only possible to generate data for the e-commerce industry. With built-in configurability, users have complete control over the generation process, allowing them to tailor the data to their specific needs.

At this stage of development, the project data is prepared only for one country - Poland.

I would like to emphasize at this stage that the **data is 100% fictional and randomly generated**. The project is intended for educational purposes only. The code included in this project is perfect for generating fictional data that can be used to practice various aspects of data analysis.

Below, in the `How can you generate the data?` section, you can find instructions on how to generate data using the code from this project.

## Features

### **1. Customer Data Generation**
   - Generates unique identifiers and personal details for customers.
   - Fields generated:
     - `customer_id`: unique customer identifier.
     - `name`, `surname`: customer's name and surname (localization options like `pl_PL`).
     - `email`: unique email address.
     - `address`: customer's address.
   - Allows configuration of the number of customers.

### **2. Product Data Generation**
   - Provides information about products, such as categories, brands, colors, and prices.
   - Fields generated:
     - `product_id`: unique product identifier.
     - `category`: product category (e.g., Electronics, Clothing).
     - `brand`: product brand.
     - `color`: product color (with options to prioritize specific colors).
     - `net_purchase_price`: net purchase price.
     - `sales_margin`: sales margin.
   - Customizable lists for categories, brands, and colors.

### **3. Sales Data Generation with Seasonality**
   - Generates sales data with the following considerations:
     - Monthly seasonality (e.g., increased sales in December).
     - Weekday seasonality (e.g., higher sales on Fridays and weekends).
     - Special periods such as Black Friday.
   - Fields generated:
     - `order_date`: date of the order.
     - `product_id`: product identifier.
     - `quantity`: number of items ordered (probabilistic distribution).
     - `customer_id`: customer identifier.
   - Customizable date range for data generation (e.g., 2022 to 2024) and year-over-year growth rate.

## How can you generate the data?

To generate the data, simply download the repository to your computer, install the required libraries from the `requirements.txt` file, and then run the `main.py` file from the main folder.

The configuration of parameters affecting the generated data is located in the `main_settings.py` file within the settings folder.

## Configuration

The generator is fully configurable, allowing users to:
1. Specify the number of customers, products, and transactions to generate.
2. Customize product categories, brands, and colors.
3. Define seasonality preferences, such as:
   - Monthly preferences (e.g., higher sales in December).
   - Weekday preferences (e.g., increased traffic on Fridays and weekends).
   - Special events like Black Friday.