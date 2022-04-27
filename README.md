# Oakland Budget Analysis J296 Final
## This is my final project for Data Journalism, J296.

### PART 01: Data Analysis – Interviewing the Data

#### QUESTION #1: Compare the overall budget from last year to this year. What was the average spent on all departments?
##### LAST YEAR
1. Highlight all cells in sheet FY21-22; Make a pivot table
2. Assign "Department" to ROWS; Assign SUM of "Amount" to VALUES
3. Copy Pivot Table, create new sheet (FY21-22 Sort Sheet) and shift+CMD+V, freeze top row and add filters
4. Click into new column, type function =AVERAGE(B2:B28)
    * TOTAL FUNDING for all departments last year: 4,066,776,078 
    * AVERAGE FUNDING for all departments last year was: 150,621,336.2

##### THIS YEAR
1. Highlight all cells in sheet FY22-23; Make a pivot table
2. Assign "Department" to ROWS; Assign SUM of "Amount" to VALUES
3. Copy Pivot Table, create new sheet (FY22-23 Sort Sheet) and shift+CMD+V, freeze top row and add filters
4. Click into new column, type function =AVERAGE(B2:B28) 
    * TOTAL FUNDING for all departments last year: 3,840,350,236
    * AVERAGE FUNDING for all departments last year was: 142,235,193.9

##### OVERALL
* There has been a nearly 150,000,000 decrease in the budget this year. The average department funding has decreased by nearly 8,000,000.

#### QUESTION #2: What departments were funded the most last fiscal year? This fiscal year? 
##### LAST YEAR
!['Pivot Table Most Funded Last Year'](/Q2FY21-22PT.png)
1. Highlight all cells in sheet FY21-22; Make a pivot table
2. Assign "Department" to ROWS; Assign SUM of "Amount" to VALUES
3. Copy Pivot Table, create new sheet (FY21-22 Sort Sheet) and shift+CMD+V, freeze top row and add filters
4. Sort SUM of AMOUNT column from Z - A
  * The five departments with the most funding were Non-Departmental, Finance, Oakland Public Works, Police, and Capital Improvement Projects. 
  * Of these five, three (Non-Departmental, Finance, and Police) departments work to serve the government. The Non-Departmental funds go towards expenses that apply to all departments like property, insurance, etc. The Finance Department takes care of all city finances. While the police do provide some services to the public, they ultimately protect city interests – not the public good. (TOTAL: 2,310,756,641 or 56.82% of total budget)
  * Only two departments in the top five have funds that directly go towards bettering Oakland for the public – Public Works and Capital Improvement Projects both of which work to fix infrastructure and better public spaces in the city. (TOTAL: 612,925,987 or 15.07% of total budget)

##### THIS YEAR
!['Pivot Table Most Funded This Year'](/Q2FY22-23PT.png)
1. Highlight all cells in sheet FY22-23; Make a pivot table
2. Assign "Department" to ROWS; Assign SUM of "Amount" to VALUES
3. Copy Pivot Table, create new sheet (FY22-23 Sort Sheet) and shift+CMD+V, freeze top row and add filters
4. Sort SUM of AMOUNT column from Z - A
  * The five departments with the most funding were still Non-Departmental, Finance, Oakland Public Works, Police, and Capital Improvement Projects. 
  * Of these five, three (Non-Departmental, Finance, and Police) departments work to serve the government and its daily functions. (TOTAL: 2,074,929,695 or 54.03% of total budget)
  * Only two departments in the top five have funds that directly go towards bettering Oakland for the public. (TOTAL: 663,786,645 or 17.28% of total budget)

##### OVERALL
* There was a slight decrease (2.79%) in government operational spending and a slight increase (2.21%) in public works spending when comparing the top five funded departments from this year to last.

#### QUESTION #3: What departments were funded the least last fiscal year? This fiscal year? 
##### LAST YEAR
1. Go to FY21-22 Sort Sheet
4. Sort SUM of AMOUNT column from A - Z
  * The five departments with the least funding were in order: Race and Equity, Public Ethics Commission, City Auditor, Police Commission, and Mayor.
  * Of these five, four (Race & Equity, Public Ethics Commission, City Auditor, and Police Commission) departments provide independent or civillian oversight into the city government. (TOTAL: 9,498,089 or .23% of total budget)
  * The Mayor is the last department receiving funding. (TOTAL: 4,790,346 or .12% of total budget)

##### THIS YEAR
1. Go to FY22-23 Sort Sheet
4. Sort SUM of AMOUNT column from A - Z
  * The five departments with the most funding were in order: Race and Equity, Public Ethics Commission, City Auditor, Mayor, and Police Commission. 
  * Of these five, four (Race & Equity, Public Ethics Commission, City Auditor, and Police Commission) departments work to check the government and provide oversight into its actions. (TOTAL: 11,182,608 or .29% of total budget)
  * The mayor's office received more funding this year. (TOTAL: 4,936,318 or .13% of total budget)

##### OVERALL
* There was a slight increase (.6%) in government oversight operations and a slight increase (.1%) in the funding that the mayor's office received. It is interesting to me that the least funded departments provide oversight into the city's most powerful agencies.

#### QUESTION #4: Compare the revenue vs expenses of each department funded LAST year and list any departments that have a large disparity between the two.
##### REVENUES
!['Pivot Table Revenue Last Year'](/Q4FY21-22RevenuePT.png)
1. Go to sheet FY21-22, highlight all cells and create a pivot table (FY21-22Revenue PT).
2. Assign "Department" to ROWS; Assign SUM of "Amount" to VALUES and set to % of Grand Total; Filter for Revenue ONLY according to account-type
    * DEPARTMENTS THAT BROUGHT IN SIGNIFICANT REVENUE
     * Finance	brought in 39.84% 
     * Non-Departmental and Port brought in 24.88% 
     * Oakland Public Works	brought in 10.44% 
     * Capital Improvement Projects brought in 4.80% 
     * Human Services	brought in 4.08% 
     * Transportation brought in 3.73%
     * Housing and Community Development brought in	3.34% 
     * Planning and Building brought in	2.70% 
 
##### EXPENSES
!['Pivot Table Expenses Last Year'](/Q4FY21-22ExpensePT.png)
1. Go to sheet FY21-22, highlight all cells and create a pivot table (FY21-22Expense PT.
2. Assign "Department" to ROWS; Assign SUM of "Amount" to VALUES and set to % of Grand Total; Filter for Expenses ONLY according to account-type
    * DEPARTMENTS WITH SIGNIFICANT EXPENSES
     * Non-Departmental and Port expensed 30.19% 
     * Police	expensed 16.52%
     * Fire	expensed 9.42%
     * Oakland Public Works expensed	8.68% 
     * Capital Improvement Projects expensed 6.22%  
     * Human Services expensed	5.49%
     * Transportation	expensed 3.75%
     * Housing and Community Development expensed	3.11%
     * Oakland Public Library expensed 2.25%
 
##### OVERALL
I notice that of the two lists (of departments with signifant spending and revenues) there are three departments that do not bring in any or much revenue but who do spend a lot of government funding. These departments are Police (16.52% of the budget used), Fire (9.42% of the budget used) and Oakland Public Library (2.25 of the budget used). Of these three departments, only the Police force is spending much more than it is actually generating revenue for the city. This is a big disparity.

#### QUESTION #5: Compare the revenue vs expenses of each department funded THIS year and list any departments that have a large disparity between the two.
##### REVENUES
!['Pivot Table Revenue This Year'](/Q5FY22-23RevenuePT.png)
1. Go to sheet FY22-23, highlight all cells and create a pivot table (FY22-23Revenue PT).
2. Assign "Department" to ROWS; Assign SUM of "Amount" to VALUES and set to % of Grand Total; Filter for Revenue ONLY according to account-type
    * DEPARTMENTS THAT BROUGHT IN SIGNIFICANT REVENUE
     * Finance brought in	44.54% 
     * Non-Departmental and Port brought in 18.42% 
     * Oakland Public Works brought in 11.02% 
     * Capital Improvement Projects	brought in 6.32% 
     * Transportation	brought in 4.14% 
     * Human Services	brought in 3.93%  
     * Planning and Building brought in	2.68% 
     * Housing and Community Development brought in	2.07%  
 
##### EXPENSES
!['Pivot Table Expenses This Year'](/Q5FY22-23ExpensePT.png)
1. Go to sheet FY22-23, highlight all cells and create a pivot table (FY22-23Expense PT.
2. Assign "Department" to ROWS; Assign SUM of "Amount" to VALUES and set to % of Grand Total; Filter for Expenses ONLY according to account-type
    * DEPARTMENTS WITH SIGNIFICANT EXPENSES
     * Non-Departmental and Port expensed	24.84% 
     * Police	expensed 17.83% 
     * Fire expensed 10.51% 
     * Oakland Public Works	expensed 9.26% 
     * Capital Improvement Projects expensed 7.97% 
     * Human Services expensed 5.40%  
     * Transportation expensed 4.18% 
     * Oakland Public Library expensed 2.41% 
     * Information Technology expensed 2.05%  
     * Planning and Building	expensed 2.05% 
     * Finance expensed	2.02% 
 
##### OVERALL
Of the significant expenses vs revenue this year, I notice a similar pattern from last year. There are four departments that do not bring in any or much revenue but who do spend a lot of government funding. These departments are Police (17.83% of the budget used), Fire (10.51% of the budget used), Oakland Public Library (2.41 of the budget used), and Information Technology (2.05% of the budget used). Of these three departments, only the Police force is spending much more than it is actually generating revenue for the city. This is a big disparity, again.

This time, in fact, the police force has more than a 1% increase in their expenses. So does the fire department. 
