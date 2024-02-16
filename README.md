# Crowdfunding Data Project - README Summary

## Project Overview

This Python-based project aims to extract, transform, and load crowdfunding data into well-structured CSV files. The primary data sources are the 'crowdfunding.xlsx' and 'contacts.xlsx' files, and the resulting outputs include 'category.csv,' 'subcategory.csv,' 'campaign.csv,' and 'contacts.csv.'

## Crowdfunding Data Extraction

The project begins by reading data from the 'crowdfunding.xlsx' file into a Pandas DataFrame (`crowdfunding_info_df`). Initial exploration of the dataset reveals essential information such as column names, data types, and non-null counts.

## Category and Subcategory DataFrames

1. **Category DataFrame**
   - A 'category.csv' file is created with columns "category_id" and "category."
   - The "category_id" is sequentially numbered from 1 to the length of unique categories.

2. **Subcategory DataFrame**
   - A 'subcategory.csv' file is created with columns "subcategory_id" and "subcategory."
   - The "subcategory_id" is sequentially numbered from 1 to the length of unique subcategories.

## Campaign DataFrame

3. **Campaign DataFrame**
   - A 'campaign.csv' file is generated with columns including "cf_id," "contact_id," "company_name," "description," "goal," "pledged," "outcome," "backers_count," "country," "currency," "launch_date," "end_date," "category_id," and "subcategory_id."
   - Data types are appropriately adjusted, and columns like "launch_date" and "end_date" are converted to datetime format.
   - The DataFrame is merged with the Category and Subcategory DataFrames to include corresponding category and subcategory names.

## Contacts DataFrame

4. **Contacts DataFrame**
   - A 'contacts.csv' file is created from the 'contacts.xlsx' file.
   - Columns include "contact_id," "first_name," "last_name," and "email."

## Project Structure

The project is organized into sections, each focusing on a specific aspect of data extraction, transformation, or loading. Code comments provide insights into the purpose and functionality of each code block. CSV files are exported to the "Resources" folder for ease of access.
