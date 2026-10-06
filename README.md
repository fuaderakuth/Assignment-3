# Power BI Assignment-3
## Data Transformation and Data Modeling

#### 1. Import Data 
  *  Imported "List of Orders.csv" file to Power Bi via Get data > CSV/Text file.
  *  “Order Details.csv” and “Sales target.csv” files were directly imported to Power Query editor via "Home" ribbons "New Source" Selection.

#### 2. Data Transformation.
  * Restricted the "List of Orders" table to only show the first 500 rows as Home> Keep Rows > Specified Number of rows as 500.
  * “Order Date” column in the “List of Orders” table is set to data type 'Date' via using Locale.
  * Changed the data type of “Amount” and “Target” columns to ‘Fixed Decimal Number’ from the column header.
  * Customer Column formatted into proper case via Ribbon Transform > Format > Capitalize Each Word.
  * Merged columns "City" and "State" via ribbon "Add Column"> Merge Columns by using CTRL + selecting "City' then "State" to display the location as instructed.
  * A new custom calculated column "Profit Margin" is created via ribbon "Add Column > Custom Column".
  * A new conditional column "Profit Status" was created via riboon "Add Column > Conditional Column".

- 1. Merging Data (Joins):
    * Merged two tables " List of Orders" and "Order Details" via Home ribbons > Merge Query > Merge Queries as new".

- 2. Handling Missing Data & Duplicate Data:
    * Checked and reviewed for any missing values via Column Filter, Column Quality and Column Statistics ( Column Profile). No action taken since no missing values found. If there were any missing values found, action would be taken as per the column data type, like if its numerical field, the missing value would be replaced by null or 0, likewise the text field would be replaced by mode of the column or "Unknown" case to case.
    *  No duplicates found. A duplicate of the table has been created in order to check duplicate values via Home ribbon > Keep Rows > Keep Duplicates. Incase if there were any duplicates found it will be removed.

- 3. Sorting and Filtering Data:
    * In the "Orders Data" table, the column "Order Date" has been sorted in Descending order via column header.
    * likewise, state "Tamil Nadu" has been filtered from the State column
    
- 4. Grouping and Aggregating Data:
    * Order Details table were duplicated by right clicking on the table, grouped as per the instruction via Home ribbon > "Group By" in Transform group > Advanced > Selected Category in the "Group" and mentioned the count, Average and Sum in the "Aggregation".
    
#### 3. Data Modeling
  * Established relationship by dragging the "Order ID" field of "Orders Details" table to Order ID field of " List of Orders" table.
  * Established relationship by dragging the "Category" field of "Orders Details" table to "Category" field of "Sales Target" table and made sure the relatioship is active via relationship management ( Properties ).
