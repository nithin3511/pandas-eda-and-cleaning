# Customer Call List Data Cleaning Using Pandas

## Project Overview

This project focuses on cleaning and transforming a raw customer contact dataset using Python and Pandas. The original dataset contained duplicate records, inconsistent phone number formats, unstructured address information, missing values, and customer records that were not suitable for outreach activities.

The objective was to convert the raw dataset into a clean, standardized, and analysis-ready customer contact list that could be used for CRM systems, reporting, or marketing campaigns.

---

## Dataset Information

**Dataset:** Customer Call List.xlsx

### Features

* CustomerID
* First_Name
* Last_Name
* Phone_Number
* Address
* Paying Customer
* Do_Not_Contact
* Not_Useful_Column

### Data Quality Issues Identified

* Duplicate customer records
* Inconsistent phone number formats
* Unstructured address information
* Special characters in customer names
* Missing values represented in multiple formats
* Unnecessary columns
* Customers marked as "Do Not Contact"

---

## Tools and Technologies

* Python
* Pandas
* OpenPyXL
* Jupyter Notebook

---

## Data Cleaning Process

### 1. Duplicate Removal

Removed duplicate customer records using Pandas to ensure data accuracy and prevent duplicate outreach.

### 2. Column Optimization

Dropped irrelevant columns that did not contribute to business analysis or customer communication processes.

### 3. Name Standardization

Cleaned customer names by removing unwanted characters such as digits, periods, underscores, and other special symbols.

### 4. Phone Number Formatting

Standardized phone numbers into a consistent format (XXX-XXX-XXXX) using regular expressions, making the dataset suitable for communication and CRM integration.

### 5. Address Transformation

Split the combined address field into:

* Street Address
* State
* Zip Code

This improved data usability for reporting and location-based analysis.

### 6. Categorical Data Standardization

Converted Yes/No values into a consistent Y/N format across customer status fields.

### 7. Missing Value Handling

Identified and standardized missing values represented as both NaN and "N/a" to maintain consistency throughout the dataset.

### 8. Business Rule Implementation

Applied business requirements by:

* Removing customers marked as "Do Not Contact"
* Removing records without valid phone numbers

### 9. Final Dataset Preparation

Reset indexes and produced a clean, structured dataset ready for downstream business use.

---

## Key Outcomes

* Improved overall data quality and consistency
* Eliminated duplicate and invalid records
* Standardized customer contact information
* Enhanced dataset usability for CRM and marketing operations
* Created a clean and business-ready customer database

---

## Skills Demonstrated

* Data Cleaning
* Data Transformation
* Data Validation
* Missing Value Handling
* Regular Expressions (Regex)
* String Manipulation
* Business Rule Implementation
* Pandas Data Analysis

---

## Project Result

Successfully transformed a messy customer contact dataset into a clean, standardized, and contact-ready customer database suitable for CRM imports, customer outreach campaigns, and further business analysis.
