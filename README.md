#  Customer Shopping Behavior Analysis

# Overview
This project analyzes customer shopping behavior to identify purchasing patterns, customer segments, and factors influencing purchase behavior.
The project follows an end-to-end data analytics workflow, including **data loading, exploratory data analysis (EDA), data cleaning and transformation using Python, SQL analysis using MySQL, and dashboard creation using Power BI**.
The goal is to transform raw customer data into meaningful insights that can support better business and customer-related decisions.

## Dataset
The project uses a **Customer Shopping Behavior** dataset containing customer demographic, purchasing, review, discount, and shopping frequency information.
Key columns include:
* Customer demographics such as Age and Gender
* Category
* Purchase Amount
* Review Rating
* Frequency of Purchases
* Discount Applied
* Promo Code Used
* Other customer shopping attributes
The dataset was initially loaded into Python using Pandas for exploration and preparation.

##  Tools & Technologies
* **Python** – Data loading, EDA, cleaning, and transformation
* **Pandas** – Data manipulation and analysis
* **MySQL** – SQL-based data analysis
* **SQLAlchemy / PyMySQL** – Connecting Python with MySQL
* **Power BI** – Interactive dashboard and data visualization
* **Jupyter Notebook** – Python analysis
* **GitHub** – Project documentation and version control


##  Project Steps
# 1. Data Loading
The customer shopping dataset was loaded into Python using Pandas.
df = pd.read_csv("customer_shopping_behavior.csv")

# 2. Exploratory Data Analysis
Initial analysis was performed to understand the dataset using:
* head()
* info()
* describe()
* Missing-value analysis
* Column and data-type inspection
* Unique-value analysis

# 3. Data Cleaning & Transformation
Several preprocessing steps were performed:
* Checked for missing values.
* Filled missing **Review Rating** values using the median rating within each product category.
* Standardized column names to lowercase.
* Replaced spaces in column names with underscores.
* Renamed `purchase_amount_(usd)` to `purchase_amount`.
* Created an **Age Group** column using age quartiles.
* Created a **Purchase Frequency Days** column by converting purchase-frequency categories into numerical days.
* Removed the `promo_code_used` column after checking its relationship with `discount_applied`.

# 4. MySQL Analysis
The cleaned dataset was loaded into a MySQL database using SQLAlchemy and PyMySQL.The cleaned data was stored in the mytable table within the customers_behaviour database.SQL queries were then used to analyze customer purchasing behavior and generate business insights.

# 5. Power BI Dashboard
The analyzed data was used to create an interactive Power BI dashboard.The dashboard presents key customer and purchasing metrics through:
* KPI cards
* Charts
* Category analysis
* Customer segmentation
* Purchase behavior analysis

# 6. Analytical Report
The final insights were organized into a structured report covering the major findings from the Python, SQL, and Power BI analysis.

# 7. Results & Key Insights
The analysis was used to identify patterns in customer purchasing behavior, including:
* Customer distribution across different age groups.
* Purchasing patterns across product categories.
* Customer purchase frequency.
* Purchase amount trends.
* Review rating patterns.
* Relationship between discounts and customer purchases.
* Differences in shopping behavior across customer segments.
The Power BI dashboard presents these findings in an easy-to-understand format for business analysis and decision-making.

##  Skills Demonstrated
* Data Cleaning
* Exploratory Data Analysis (EDA)
* Data Transformation
* Python
* Pandas
* SQL
* MySQL
* Power BI
* Data Visualization
* Customer Behavior Analysis
* Business Intelligence
* Data Storytelling


