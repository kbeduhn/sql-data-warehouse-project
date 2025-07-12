


## General Principles
- **Naming Conventions:** Use snake_case with lowercase letters and underscores (_) to separate words.
- **Language:** Use English for all names.
- **Avoid Reserved Words:** Do not use SQL reserved words as object names. 

## Table Naming Conventions

### Bronze Rules
- All names must start with the source system name, and table names must match their original names without renaming.
- **<sourcsystem>_<entity>**
    - <sourcesystem>: Name of the source system (e.g., crm, erp).
    - <entity>: Exact table name from the source system.
    - Example: crm_customer_info -> Customer information from the CRM system.

### Silver Rules
- All names must start with the source system name, and table names must match their original names without renaming.
- **<sourcsystem>_<entity>**
    - <sourcesystem>: Name of the source system (e.g., crm, erp).
    - <entity>: Exact table name from the source system.
    - Example: crm_customer_info -> Customer information from the CRM system.

### Gold Rules
- All names must use meaningful, business-aligned names for tables, starting with the category prefix.
- **<category>_<entity>**
    - <category>: Describes the role of the table, such as dim (dimension) or fact (fact table).
    - <entity>: Descriptive name of the table, aligned wiht the business domain (e.g., customers, products, sales).
    - Examples;
        - dim_customers -> Dimension table for customer data.
        - fact_sales -> Fact table containing sales transactions.
     
#### Glossary of Category Patterns
| Pattern | Meaning | Example(s)|
|---------|---------|-----------|
| dim | Dimension table | dim_customer, dim_product|
| fact | Fact table | fact_sales |
| agg_ | Aggregated table | agg_customers, agg_sales_monthly |

## Column Naming Conventions

### Surrogate Keys
- All primary keys in dimension tables must use the suffix _key.
- <table_name>: Refers to the name of the table or entity the key belongs to.
- _key: A suffix indicating that this column is a surrogate key.
-  Example: customer_key _> Surrogate key in the dim_customers table.

## Stored Procedure
- All stored procedures used for loading data must follow the naming pattern: load_<layer>/
  


























