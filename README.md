# pandas-eda-and-cleaning
**Customer Call List — Data Cleaning Project**

A data cleaning project in pandas that transforms a messy customer contact list — inconsistent phone formats, stray punctuation, combined address fields, duplicates, and irregular missing-value representation — into a clean, standardized, and contact-ready dataset.

Dataset
File: Customer Call List.xlsx
Columns: CustomerID, First_Name, Last_Name, Phone_Number, Address, Paying Customer, Do_Not_Contact, Not_Useful_Column
Issues in the raw data: duplicate rows, phone numbers in multiple inconsistent formats, names with leading/trailing junk characters, a single address field combining street/state/zip, and missing values represented inconsistently (NaN and the string "N/a").


Tools & Libraries:
Python 3
pandas
openpyxl (for reading .xlsx files)


Cleaning Workflow:-
Remove duplicates — drop_duplicates() to eliminate exact duplicate rows.
Drop irrelevant columns — removed Not_Useful_Column.
Clean names — stripped stray leading/trailing characters from Last_Name (digits, periods, underscores, slashes).
Standardize phone numbers — removed all non-alphanumeric characters via regex, then reformatted into a consistent XXX-XXX-XXXX pattern, cleaning up leftover artifacts from missing values along the way.
Split address field — separated the combined Address column into Street_Address, State, and Zip_code.
Standardize categorical flags — converted Yes/No values to Y/N in Paying Customer and Do_Not_Contact.
Unify missing values — replaced both NaN and the literal string "N/a" with a consistent blank representation.
Apply business rules — removed customers flagged Do_Not_Contact, and removed customers with no usable phone number.
Reset index — produced a clean, sequentially indexed final dataset.


Result:-
A deduplicated, standardized customer list containing only contactable, opted-in customers, with consistent name formatting, phone number formatting, and split address fields ready for downstream use (e.g. a CRM import or an actual outreach call list).
