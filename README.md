# Oakland Budget Analysis J296 Final
## PART 02: Data Analysis – Interviewing the Data

### QUESTION #1: Compare the overall budget from last year to this year. What was the average spent on all departments?
#### LAST YEAR
!['Overall Budget Last Year'](/Q1PTFY21-22.png)
1. Highlight all cells in sheet FY21-22; Make a pivot table
2. Assign "Department" to ROWS; Assign SUM of "Amount" to VALUES, filter by Account-Type (Expenses only)
3. Copy Pivot Table, create new sheet (FY21-22 Sort Sheet) and shift+CMD+V, freeze top row and add sort option
4. Click into new column, type function =AVERAGE(B2:B28)
    * TOTAL FUNDING for all departments last year: 2,033,463,039 
    * AVERAGE FUNDING for all departments last year was: 75,313,446

#### THIS YEAR
!['Overall Budget This Year'](/Q1PTFY22-23.png)
1. Highlight all cells in sheet FY22-23; Make a pivot table 
2. Assign "Department" to ROWS; Assign SUM of "Amount" to VALUES, filter by Account-Type (Expenses only)
3. Copy Pivot Table, create new sheet (FY22-23 Sort Sheet) and shift+CMD+V, freeze top row and add sort option
4. Click into new column, type function =AVERAGE(B2:B28) 
    * TOTAL FUNDING for all departments last year: 1,920,271,118
    * AVERAGE FUNDING for all departments last year was: 71,121,153

#### OVERALL
* There has been over 100,000,000 decrease (113,191,921) in the budget this year. The average department funding has decreased by nearly 4,000,000.

### QUESTION #2: Compare the difference between the overall expenses vs. revenues for the budget from last year to this year.
#### LAST YEAR
!['Overall Deficit Last Year'](/Q2PTFY21-22.png)
1. Highlight all cells in sheet FY21-22; Make a pivot table
2. Assign "Department" to ROWS; Assign SUM of "Amount" to VALUES; Assign "Column" to Account-Type
3. Copy Pivot Table, create new sheet (FY21-22 Q2 Sort Sheet) and shift+CMD+V, freeze top row and add sort option
4. Click into new column, type function =C29-B29 (where C29 = grand total of revenue and B29= grand total of expenses)
   * In FY21-22, the city of Oakland went over their budget by $150,000.
    

#### THIS YEAR
!['Overall Deficit This Year'](/Q2PTFY22-23.png)
1. Highlight all cells in sheet FY22-23; Make a pivot table
2. Assign "Department" to ROWS; Assign SUM of "Amount" to VALUES; Assign "Column" to Account-Type 
3. Copy Pivot Table, create new sheet (FY22-23 Q2 Sort Sheet) and shift+CMD+V, freeze top row and add sort option
4. Click into new column, type function =C29-B29 (where C29 = grand total of revenue and B29= grand total of expenses)
    * In FY22-23, the city of Oakland went over their budget by $192,000.

#### OVERALL
* The city has been better about staying within budget but there are still departments that are overspending.

### QUESTION #3: What departments were funded the most last fiscal year? This fiscal year? 
#### LAST YEAR
1. Go to FY21-22 Q2 Sort Sheet
4. Sort SUM of EXPENSES column from Z - A
  * The five departments with the most funding were Non-Departmental, Police, Fire, Oakland Public Works and Capital Improvement Projects.
  * Of these five, two (Non-Departmental and Police) departments work to serve the government. The Non-Departmental funds go towards expenses that apply to all departments like property, insurance, etc. While the police do provide some services to the public, they ultimately protect city interests – not the public good. (TOTAL: 949,693,403 or 47% of total budget)
  * Three departments in the top five have funds that directly go towards bettering Oakland for the public – Fire, Public Works, and Capital Improvement Projects. The Fire department serves as emergency personnel in fire and other emergency situations. Public Works and CIP both work to fix infrastructure and better public spaces in the city. (TOTAL: 494,457,474 or 24% of total budget)

#### THIS YEAR
1. Go to FY22-23 Q2 Sort Sheet
4. Sort SUM of EXPENSES column from Z - A
  * The five departments with the most funding were still Non-Departmental, Police, Fire, Oakland Public Works and Capital Improvement Projects.
  * Of these five, two (Non-Departmental and Police) departments work to serve the government. (TOTAL: 819,303,567 or 43% of total budget)
  * Three departments in the top five have funds that directly go towards bettering Oakland for the public – Fire, Public Works, and Capital Improvement Projects. (TOTAL: 532,770,245 or 28% of total budget)

#### OVERALL
* There was a slight decrease (3%) in government operational spending and a slight increase (4%) in public works spending when comparing the top five funded departments from this year to last.

### QUESTION #4: What departments were funded the least last fiscal year? This fiscal year? 
#### LAST YEAR
1. Go to FY21-22 Q2 Sort Sheet
4. Sort SUM of EXPENSES column from A - Z
  * The five departments with the least funding were in order: Race and Equity, Public Ethics Commission, City Auditor, Police Commission, and Workplace and Employment Standards.
  * Of these five, all departments provide independent or civillian oversight into the city government. (TOTAL: 1,116,622 or .05% of total budget)

#### THIS YEAR
1. Go to FY22-23 Q2 Sort Sheet
4. Sort SUM of EXPENSES column from A - Z
  * The five departments with the most funding were in order: Race and Equity, Public Ethics Commission, City Auditor, Mayor, and Workplace and Employment Standards. 
  * Of these five, four (Race & Equity, Public Ethics Commission, City Auditor, and Workplace and Employment Standards) departments work to check the government and provide oversight into its actions. (TOTAL: 6,508,737 or .34% of total budget)
  * The mayor's office was the last department in this list. (TOTAL: 4,936,318 or .26% of total budget)

#### OVERALL
* There was a slight increase (.3%) in government oversight operations and a slight decrease in the funding that the mayor's office received (.02%). It is interesting to me that the least funded departments provide oversight into the city's most powerful agencies.

### QUESTION #5: Compare the revenue vs expenses of each department funded LAST year and list any departments that have a large disparity between the two.
#### REVENUES
!['Pivot Table Revenue Last Year'](/Q4FY21-22RevenuePT.png)
1. Go to sheet FY21-22, highlight all cells and create a pivot table (FY21-22Revenue PT).
2. Assign "Department" to ROWS; Assign SUM of "Amount" to VALUES and set to % of Grand Total; Filter for Revenue ONLY according to account-type
    * DEPARTMENTS THAT BROUGHT IN SIGNIFICANT REVENUE
     * Finance	brought in 39.84% 
     * Non-Departmental and Port brought in 24.88% 
     * Oakland Public Works brought in 10.44% 
     * Capital Improvement Projects brought in 4.80% 
     * Human Services brought in 4.08% 
     * Transportation brought in 3.73%
     * Housing and Community Development brought in	3.34% 
     * Planning and Building brought in 2.70% 
 
#### EXPENSES
!['Pivot Table Expenses Last Year'](/Q4FY21-22ExpensePT.png)
1. Go to sheet FY21-22, highlight all cells and create a pivot table (FY21-22Expense PT.
2. Assign "Department" to ROWS; Assign SUM of "Amount" to VALUES and set to % of Grand Total; Filter for Expenses ONLY according to account-type
    * DEPARTMENTS WITH SIGNIFICANT EXPENSES
     * Non-Departmental and Port expensed 30.19% 
     * Police expensed 16.52%
     * Fire	expensed 9.42%
     * Oakland Public Works expensed 8.68% 
     * Capital Improvement Projects expensed 6.22%  
     * Human Services expensed 5.49%
     * Transportation expensed 3.75%
     * Housing and Community Development expensed	3.11%
     * Oakland Public Library expensed 2.25%
 
#### OVERALL
I notice that of the two lists (of departments with signifant spending and revenues) there are three departments that do not bring in any or much revenue but who do spend a lot of government funding. These departments are Police (16.52% of the budget used), Fire (9.42% of the budget used) and Oakland Public Library (2.25% of the budget used). Of these three departments, only the Police force and Fire department are spending much more than they are  actually generating revenue for the city. However I think it is important to note how the climate crisis (and worsening wildfires) are coming into play here. It is also important to note that the Police Department is expensing nearly twice as much as the Fire Dept. This is a big disparity.

### QUESTION #6: Compare the revenue vs expenses of each department funded THIS year and list any departments that have a large disparity between the two.
#### REVENUES
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
 
#### EXPENSES
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
 
#### OVERALL
Of the significant expenses vs revenue this year, I notice a similar pattern from last year. There are four departments that do not bring in any or much revenue but who do spend a lot of government funding. These departments are Police (17.83% of the budget used), Fire (10.51% of the budget used), Oakland Public Library (2.41% of the budget used), and Information Technology (2.05% of the budget used). Of these three departments, only the Police force is spending much more than it is actually generating revenue for the city. This is a big disparity, again.

This time, in fact, the police force has more than a 1% increase in their expenses. So does the fire department. 
