# Project2

# Crowdfunding_ETL

This code is designed to extract data from a crowdfunding.xlsx file and perform various operations on the data using the Pandas library in Python. Below is an overview of the code and its functionality:

1. Importing Dependencies
The code starts by importing the necessary dependencies, including Pandas and NumPy libraries.

2. Extracting Data
The code reads the data from the 'crowdfunding.xlsx' file into a Pandas DataFrame called crowdfunding_info_df.

3. Creating Category and Subcategory DataFrames
The code creates two DataFrames, category_df and subcategory_df, based on the unique categories and subcategories extracted from the crowdfunding_info_df. These DataFrames are then exported as CSV files, 'category.csv' and 'subcategory.csv', respectively.

4. Working with Categories and Subcategories
The code retrieves the unique categories and subcategories from the DataFrames and stores them in lists. It then prints the lists and their lengths.

5. Creating Category and Subcategory IDs
The code creates numpy arrays for category IDs (category_ids) ranging from 1 to 9 and subcategory IDs (subcategory_ids) ranging from 1 to 24. It also prints the arrays.

6. Adding Prefixes to Category and Subcategory IDs
The code uses list comprehensions to add prefixes to each category ID and subcategory ID. The modified lists are then printed.

7. Creating Category and Subcategory DataFrames
The code creates two DataFrames, category_df and subcategory_df, using the modified category and subcategory lists. These DataFrames contain the category/subcategory IDs and names. The DataFrames are printed.

8. Exporting Category and Subcategory DataFrames
The code exports the category_df and subcategory_df DataFrames as CSV files, 'category.csv' and 'subcategory.csv', respectively.

9. Creating a Campaign DataFrame
The code creates a copy of the original DataFrame, crowdfunding_info_df, called campaign_df. It then performs various transformations on the columns of the DataFrame, including renaming columns, converting data types, and formatting date columns.

10. Merging Campaign DataFrame with Category and Subcategory DataFrames
The code merges the campaign_df DataFrame with the category_df DataFrame on the 'category' column and the subcategory_df DataFrame on the 'subcategory' column. The resulting DataFrame, campaign_merged_df, contains additional columns for 'category_id' and 'subcategory_id'.

11. Exporting Campaign DataFrame
The code exports the campaign_merged_df DataFrame as a CSV file, 'campaign.csv'.
