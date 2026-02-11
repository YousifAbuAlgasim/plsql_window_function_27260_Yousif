# plsql_window_function_27260_Yousif


# Simba Supermarket Sales Analysis Project

## 1. Business Problem

### Business Context
Simba Supermarket operates in different cities in Rwanda and sells food and household products.

### Data Challenge
The management does not clearly know which products generate the highest sales in each city and how sales change over time.

### Expected Outcome
Use SQL analysis to improve inventory planning and marketing strategies.

---

## 2. Success Criteria

1. Identify top 5 products using RANK().
2. Calculate running monthly sales using SUM() OVER().
3. Compare monthly sales using LAG().
4. Segment customers using NTILE(4).
5. Calculate moving averages using AVG() OVER().

---

## 3. Database Schema D

<img width="1536" height="1024" alt="Database Schema Diagram" src="https://github.com/user-attachments/assets/5e902b43-c20d-4f32-94a6-95f410ad6a3b" />




**4. SQL JOIN Queries**

**Display Complete Sales Information**

<img width="933" height="870" alt="Screenshot 2026-02-08 203609" src="https://github.com/user-attachments/assets/6c0843a6-b3fe-4ba5-ae49-c872134263e4" /> 
.
.

**Identify Customers Without Sales**
<img width="928" height="871" alt="image" src="https://github.com/user-attachments/assets/bf770603-ef60-413e-9bdb-4ca29ae927c6" />
.
.

**Compare Customers in the Same Cit**
<img width="935" height="876" alt="image" src="https://github.com/user-attachments/assets/a1e6a9d1-55ac-43ca-ae07-d6f91400abfe" />

.



## 5. Window Functions

1 Ranking Function 
<img width="930" height="879" alt="image" src="https://github.com/user-attachments/assets/8597aa6d-a4b5-4b42-b392-6c3a4e1fe06b" />


2 Aggregate Function – SUM() OVER() (Running Total)
<img width="935" height="877" alt="image" src="https://github.com/user-attachments/assets/45762e38-e21b-43d0-b7e0-29d4b2771c5e" />


3 Navigation Function – LAG() (Month-to-Month Comparison)
<img width="931" height="874" alt="Screenshot 2026-02-08 204448" src="https://github.com/user-attachments/assets/56fb633d-d53c-46a0-87b0-5959fc2fdb58" />



4 Distribution Function – NTILE(4) (Customer Segmentation)
<img width="933" height="874" alt="image" src="https://github.com/user-attachments/assets/a2862dde-2d78-4ed8-a1bf-2e28fb44db01" />



5 Moving Average – AVG() OVER() (Three-Month Average)
<img width="936" height="873" alt="image" src="https://github.com/user-attachments/assets/ee3f7b89-5719-4bb0-ada4-a884ed337148" />


 6. Results Analysis

### Descriptive
The analysis shows that sales are higher in Kigali compared to other cities.
Certain products, such as food items, generate more revenue than hygiene and cleaning products.
Monthly sales records indicate a steady increase during the first quarter of 2025.

Interpretation

Most customers prefer basic household and food products, leading to higher sales in these categories.

### Diagnostic
Description

Higher sales in Kigali are mainly due to higher population density and stronger commercial activities.
Customers in urban areas tend to have higher purchasing power and more frequent shopping habits.

Interpretation
Better product availability, accessibility, and customer traffic in major cities contribute to increased sales.
### Prescriptive
Description
Simba Supermarket should increase inventory levels for top-selling products in high-performing cities.
Marketing campaigns should focus on inactive and low-spending customers.

Recommendations
-Increase stock for high-demand products in Kigali and other major cities.
-Offer discounts and loyalty programs to low-activity customers.
-Expand popular product categories in high-revenue branches.
-Monitor monthly sales trends regularly using window functions.



## 7. References

Oracle Corporation. (2023). Oracle Database SQL Language Reference – Analytic (Window) Functions.
https://docs.oracle.com/en/database/oracle/oracle-database/19/sqlrf/Analytic-Functions.html

Oracle Corporation. (2023). Oracle Database SQL Language Reference – SELECT and JOIN Clauses.
https://docs.oracle.com/en/database/oracle/oracle-database/19/sqlrf/SELECT.html

W3Schools. (2024). SQL JOIN Tutorial.
https://www.w3schools.com/sql/sql_join.asp

W3Schools. (2024). SQL Window Functions.
https://www.w3schools.com/sql/sql_window_functions.asp

GeeksforGeeks. (2024). SQL Window Functions.
https://www.geeksforgeeks.org/window-functions-in-sql/

Course Lecture Slides – Database Development with PL/SQL (INSY 8311), AUCA, 2026.
---

All sources were properly cited. Implementations and analysis represent original work.
