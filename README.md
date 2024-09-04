The purpose of this file is to demostrate the logic of the code and then the basic explaination of the specific package.
We start the task with the list of all the SPAC companies, the list is manually get from SEC.GOV EDGAR
We have use the follwing way to manually select companies;
Based on the standard industry code, we have apply the "6770" as blank check comapny code.
Then follow the list of the blank check, we have the comapny centre index key (CIK) and official name of company.
Then with CIK, we applied the SEC.GOV EDGAR api to get the TICKER for all the company, to better match the stock info for the company
The code also include the "get_filling_auto" function which is for automatic download the filling from SEC.GOV.
The goal to download the filling is to get the textual information (i.e CEO name, events info, etc,.)
About the CEO info we have applied Capital IQ for all the CEO with the list we have frm blank check, use CIK to match.
So, we have all the basic info for the dataset, Company name, CIk, CEOs, Ticker
We have use yahoo finance to get all the stock info, then we get open price and close price to calclate the return of each stock.
We have applied the events study for this task, and set the events date is CEOs replacement date.
Then for the regression part, we have use linear and logic both. 
For the variable part, we have use stock return and CEOs basic info, (i.e Age, experience year, sponsor flag, etc)
We have reached a satidified result, and we have mentioned the discussion in the thesis, about next step.
