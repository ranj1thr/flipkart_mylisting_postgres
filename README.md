# Flipkart Order Report Uploader

This script automates the upload of Flipkart detailed order reports from Excel files into a PostgreSQL database. It uses hardcoded database credentials in the script for connection.

## Setup Instructions

1. **Install Required Packages**
   ```bash
   pip install pandas sqlalchemy psycopg2 rich numpy
   ```

2. **Configure Database Credentials**
   Edit the `db_config` dictionary in the script to match your PostgreSQL credentials and database name.

3. **Run the Script**
   ```bash
   python upload_order_tab_to_postgres.py
   ```

## Notes
- The script expects Excel files to be in the folder specified by `base_path` in the script. Adjust this path as needed.

For any questions or improvements, feel free to ask!

# Flipkart My Listing to PostgreSQL

This script processes and uploads data from the Flipkart Seller Panel's "My Listing" tab to a PostgreSQL database.

## Features
- Cleans and standardizes Flipkart listing data from Excel
- Extracts FSN from listing URLs
- Handles missing values and normalizes columns
- Appends cleaned data to a PostgreSQL table

## Usage
1. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
2. Update the database connection details in the script if needed.
3. Place your Flipkart Excel export at the specified path or update the path in the script.
4. Run the script:
   ```
   python flipkart_mylisting_postgres.py
   ```

## Requirements
- Python 3.7+
- PostgreSQL database
- Flipkart Seller Panel Excel export

---
This is part of the Flipkart data tools suite.
