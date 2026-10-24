# Mini-project-1
Data cleaning using excel
# Data cleaning using excel 
## Check and correct date format
* Corrected date format by changing text formate into short date format
## Colume type changed 
* Changed the net amount and discount amount column into number format and adjusted there decimal places
## Trim and proper function
* capitalized each word form the text columns using power query
## Conditional colume
* created a conditional column for age group
  
* Table.AddColumn(#"Replaced Value", "Age catazory", each if [Age Group] = "18-25" then "Young Adult" else if [Age Group] = "25-45" then "Early Adult" else if [Age Group] = "45-60" then "Middle age " else if [Age Group] = "60 and above" then "Senior citizen" else "Teenage")
## Replaced value 
* replaced the value of **Upi** into **UPI** by means of replacing value
## Missing values
* Found blank null space in the discount name column replaced the null value with **Not applicable**
* created a conditional colume for discount name **= Table.AddColumn(#"Added Conditional Column", "Discount ", each if [Discount Availed] = "No" then "Not Applicable" else [Discount Name])**
## conditional formating
* Highlighted the rows **Not appalicable** using conditional formating
