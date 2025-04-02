# Real-Estate-Market-Analysis
**Investigating Property transactions and Customer satisfaction**

The real estate market is a complex and dynamic entity of great intrest for professionals in the field, investors, policymakers, and data analysts that wish to thorougly undersand the market conditions and customer behaviour and make informed decisions. In our Real Estate Market Analysis with Python project, the client-a leading company in the industry-has collected data on properties and their customers and wishes to gain indights with real estate analysis

## Table of Contents
- [Project Objective](#Project-Objective)
- [Data Preprocessing](#Data-Preprocessing)
  - [Data Cleaning and Preprocessing (Properties Dataset)](#Data-Cleaning-and-Preprocessing (Properties Dataset))
  - [Data Cleaning and Preprocessing (Customers Dataset)](#Data-Cleaning-and-Preprocessing (Customers Dataset))
  - [Combining the Two Datasets](#Combining-the-Two-Datasets)
- [Descriptive Statistics](#Descriptive-Statistics)
- [Data Analysis](#Data-Analysis)
- [Data Visualization](#Data-Visualization)
- [Data Interpretation](#Data-Interpretation)


## Project Objective
This project aims to preprocess, analyze, and visualize the real estate property data, therby generating meaningful insights about property transactions and customer profiles

## Data Preprocessing
1. Import all the relevant libraries
2. Read the data
3. Data Cleaning
4. Combining two datasets

### Data Cleaning and Preprocessing (Properties Dataset)
- **Create a Copy of the Original Dataset**
  
  Creating a new variable that replicates the original data acts as a natural 'checkpoint' in our data processing. This ensures that we always have access to pristine data if we need to revert our changes indicating that it holds a safeguard copy of the original data
  ```python
     properties = prop_df.copy()
  ```

- **Casting Id column to string**
  IDs are often arbitrary identifiers, not numerical values meant for calculations. Treating IDs as strings allows us to perform categorical operations like grouping data by ID, counting unique IDs,etc. Converting ID columns to strings ensures that they are treated as labels rather than numerical values.
  
- **Resolving the col_name issue**
  When we try to convert `id` column to string we encounter an error. (Pandas doesn't recognize it as a valid column name). Upon investigating we found an encoding issue with an unnecessary byte order mart(BOM) attached to the column name. The solution for this is, we rename the column, effectively discarding the irrelevant metadata
  
- **Changing the dtype of building and property# columns**
- **Dealing with date_sale column**
- **Change the case of the type column to lowercase for consistency**
- **Dealing with Price column**
- **Mapping values in status column to 1's and 0's**
- **Checking for missing values and Dealing with them if necessary**

### Data Cleaning and Preprocessing (Customers Dataset)
- **Create a Copy of the Original Dataset**
- **Inspecting column names and dealing with them if necessary**
- **Renaming the entity column and mapping values to 1's and 0's**
- **Mapping Gender values to 1's and 0's**
- **Changing the case of purpose and source columns to lower-case**
- **Mapping mortgage values to 1's and 0's**
- **Creating a full_name column by combining name and surname**
- **Changing the dtype of birth_date column**

### Combining the Two Datasets
1. **Preliminary checks**
2. **Mergeing 2 tables**
3. **Identifying and Resolving merge issues**
4. **Final checks and merge**
5. **Handling missing values**

## Descriptive Statistics
#### Breakdown by Building
#### Breakdown by Country
#### Breakdown by State

## Data Analysis
#### Analyzing customers age
#### Analysis of the price of properties
#### Relationship between age and price

## Data Visualization
#### Deal satisfaction by Country (Bar Chart)
#### Age Distribution (Histogram)
#### Segmentation by State (Pareto Chart)
#### Total sales per year (Line Chart)
#### Yearly sales distribution across buildings (Stacked Area Chart)

## Data Interpretation 
#### Customer Profile
#### Building Characteristics 

