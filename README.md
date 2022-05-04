# Oakland Budget Analysis J296 Final
## PART 01: Data Analysis – Interviewing the Data

NOTE: The datasets I used came from Open Budget Oakland. Specifically I looked at the budgets for this year and last year. They are named "DATASET_FY22-23_adopted.csv" and "DATASET_FY21-22_adopted.csv" (respectively)

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
* The city has been worse about staying within budget (by 42,000); there are still departments that are overspending.

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

## PART 02: The Story – Why Are These Oaklanders Calling For A People's Budget?
### A grassroots Oakland organization wants to change who's in charge of the city budget. 
#### By Hanisha Harjani

The late afternoon sun beats down on the parking lot’s asphalt. Tia Taruc-Myers is positioned in front of this Grocery Outlet’s automatic sliding doors; she squints towards Broadway, where cars and buses race to beat the turning colors of the traffic light, and she tries to make eye contact with people walking into the store. 

“Sign for A People’s Budget of Oakland? We just need your signature,” she calls out to them. Many of them pretend not to hear her but others are intrigued. A People’s Budget? What’s that? They pause, ask questions.

Taruc-Myers explains that it’s a way to bring direct democracy to Oakland; to let the people decide where their money goes, what it funds. The People’s Budget initiative was founded by Community Democracy Project ¬(CDP) – a grassroots organization born out of the flames of the Occupy Oakland movement.

This isn’t the first time that Taruc-Myers is gathering signatures for the initiative. This is the third time organizers are trying to get The People’s Budget on the ballot. When they first tried this in 2015, they were too slow to collect signatures and quickly realized that they wouldn’t get to the necessary 40,000 in the allotted 6 months’ time. In 2019, they were closer. This time, they had 40,000 signatures but not all of them were verified. Some Berkeley voters had signed, making their petition invalid.

But Taruc-Myers feels optimistic today. It is Wednesday, April 27th; the first day of attempt #3 at getting The People’s Budget on the Oakland City Ballot. “I think it's actually going to be easier now because of the Black Lives Matter movement and their focus on defunding the police,” says Taruc-Myers. “I think it'll be easier to help people understand how important a budget is ¬– especially locally.”

Another CDP organizer, Blake Hihara agrees. In a KPFA interview last January, he said “I’ve talked to thousands of people on the streets of Oakland, when collecting signatures for our initiative.” What Hihara realized was that “people care about safety […] good streets […] filling in those potholes [and] having a livable community. And, when we’re spending that money on police budget overtime,” he said, “we need huge systemic change.”

Police overspending is just one of the things that Hihara and other organizers point to, to showcase city budget mismanagement but it’s an effective talking point. The Oakland Police Department (OPD) is one of the highest funded city departments, routinely taking in anywhere from 16% to 21% of the total city budget. 

Additionally, unlike other city departments with a lot of expenditures, OPD does not bring in nearly the same amount of money it spends. 

!['Top 5 Funded Departments Data Viz'](/Top5FundedDataViz.png)(https://infogram.com/top-5-fy22-23-1hd12yx7ovwox6k?live)

This graph shows the vast disparity between the revenue and expenses of the Police department compared to the other five most funded departments. Nearly every single one (save the Fire and Police department) evens out spending with the revenue they bring in. In the case of the Fire department, it is also important to consider the impact that the worsening climate crisis and more frequent, more devastating wildfires are having on the department’s increased spending.

!['Policing Funding Data Viz'](/OPDFundingGraph.png)(https://infogram.com/police-vs-crime-1h7k230p3953v2x?live)
!['Crime Rates Data Viz'](/CrimeGraph.png)(https://infogram.com/police-vs-crime-1h7k230p3953v2x?live)

By comparison, based on [this data aggregated from sources like the DOJ and FBI](https://docs.google.com/spreadsheets/d/1EBNrb0qsuJLiwBCgNkl-EP2_LYo3gAvqiGRJmM_lwOE/edit#gid=0), increased police funding in Oakland has done very little to actually decrease crime rates in the area. In the case of violent crime, there has been a 4.23% increase from 2018 to 2021. Property crime has decreased by an insignificant 1% but not before seeing a sharp uptick in crime rates from 2018-2019. Coincidentally, this is the same year that OPD saw an increase in funding from $291,024,081 to $318,707,837 (a nearly 10% increase).

All of this raises the question – if increased police spending is not decreasing crime, what is the money actually doing? Hihara and Taruc-Myers point to other departments that could take on responsibilities similar to OPD. There is a department dedicated to Violence Prevention but currently, it only has funding of $27,380,953, or only 1% of the city budget. Taruc-Myers wonders what crime in Oakland might look like if some of the Police funding went to this department; or if it helped create more affordable housing, or libraries, or educational opportunities for the city’s youth.

Earlier this year, the Bay Area Council, a local advocacy group released the results of their annual [Bay Area Quality of Life Survey](https://drive.zooce.com/management/builtinapps/fileoperator.aspx?child=1&a=D3B60E43-50D3-46D5-A799-2C3CECF14238&ro=1&fid=4617797970591790573_15094471938716140981). To Rufus Jeffris, who manages communications at the Bay Area Council, the results are clear – “people in the Bay Area are grumpy,” he says.  And it’s true – a majority of residents are dissatisfied with the quality of life in the area, with 64% citing that things in the Bay Area are on the “Wrong Track”. Over 89% of respondents claimed that housing, crime, and cost of living were some of the most important problems facing the region. 

To Jeffris, the survey is an important indicator of the needs going unmet in the area. He says council conducts this survey annually to “try and gauge the general mood in the region and ask voters to help inform our policy work; the survey validates that we're focused on the right issues.”

While policy is all well and good, for Taruc-Myers, it’s not doing nearly enough. “Even if you have an awesome policy, most things need to be funded,” she says. “Without money, it won't happen.” 

She recalls another underfunded sector within the Oakland City Government–the Race and Equity department, which receives a paltry 0.06% of the city budget. “I'm sure whoever created that department had awesome policies and thought that the department would be powerful enough to do something they called equity but without the money, it's really hard to do important work. So, I focus most of my energy on the people's budget.”

And this isn’t just for herself. Taruc-Myers has a 7-week year old baby named Mia. She hopes that the work she is doing now – of gathering these signatures and imagining a better future ¬– creates a better Oakland for her daughter growing up. 

“I hope there will be libraries on every other block and places where people can gather and talk with each other comfortably. Now, this is true for some parts of Oakland but I want it for all of Oakland,” she says. 

