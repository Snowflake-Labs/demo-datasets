# Avalanche Ski Gear Company - Dataset Documentation

## Overview
This repository contains datasets for `Avalanche Inc`, a hypothetical premium ski gear company specializing in high-performance winter sports equipment. The datasets provide insights into product catalog, customer reviews, order history, and shipping logistics.

## Datasets

### 1. Product Catalog (`product-catalog-with-category-label`)
- **Description**: Comprehensive catalog of Avalanche's premium ski equipment and apparel
- **Fields**:
  - `name`: Product name
  - `description`: Detailed technical specifications and features
  - `price`: Product price in USD
  - `category`: Product category (Skis, Apparel, Accessories)
- **Products Include**:
  - Alpine Skis
  - Performance Racing Skis
  - Thermal Gloves
  - Insulated Jacket
  - Carbon Fiber Poles
  - Ski Goggles
  - Pro Ski Boots
  - Mountain Series Helmet
  - Alpine Base Layer
  - Avalanche Safety Pack

### 2. Customer Reviews (`customer_reviews`)
- **Description**: Customer feedback and sentiment analysis for Avalanche products
- **Fields**:
  - `PRODUCT`: Product name
  - `DATE`: Review date
  - `SUMMARY`: Detailed review text
  - `SENTIMENT_SCORE`: Sentiment analysis score (-1.0 to 1.0)
- **Insights**:
  - Reviews span from October 2023 to December 2023
  - Includes detailed testing feedback from various skiing conditions
  - Sentiment scores help track customer satisfaction

### 3. Order History (`order-history`)
- **Description**: Transaction records of customer purchases
- **Fields**:
  - `Order ID`: Unique order identifier
  - `Customer ID`: Unique customer identifier
  - `Product ID`: Unique product identifier
  - `Product Name`: Name of purchased product
  - `Quantity Ordered`: Number of items purchased
  - `Price`: Unit price in USD
  - `Total Price`: Total order value
  - `Date`: Order date
- **Coverage**:
  - Orders from October 15, 2023 to November 7, 2023
  - Includes 25 unique orders

### 4. Shipping Logs (`shipping-logs`)
- **Description**: Tracking information for order deliveries
- **Fields**:
  - `order_id`: Order identifier
  - `shipping_date`: Date of shipment
  - `carrier`: Shipping company
  - `tracking_number`: Package tracking number
  - `latitude`: Delivery location latitude
  - `longitude`: Delivery location longitude
  - `status`: Current shipping status
- **Carriers**:
  - SwiftWing Logistics
  - MountainRoute Express
  - AlpineSpeed Delivery
  - PeakPath Shipping
  - SnowRunner Logistics
  - SummitLine Express

## Data Relationships
- `Order History` links to Shipping Logs via `Order ID`
- `Product Catalog` provides detailed information about products referenced in `Order History`
- `Customer Reviews` provide feedback on products listed in the `Product Catalog`

## Data Quality
- All datasets are in `CSV` and `JSON` format
- Consistent date formatting (YYYY-MM-DD)
- Standardized currency format (USD)
- Complete product descriptions and specifications
- Comprehensive shipping tracking information

## Usage Notes
- Product prices are in USD
- Sentiment scores range from -1.0 (negative) to 1.0 (positive)
- Shipping coordinates are in decimal degrees
- All dates are in YYYY-MM-DD format

## Data Updates
- Product Catalog: Static (as of December 2023)
- Customer Reviews: Updated through December 2023
- Order History: Covers October-November 2023
- Shipping Logs: Tracks deliveries through November 2023 