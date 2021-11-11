# Files And Access 

### CRM Portal
CRM URL : https://crm-simulator.vercel.app/

Username: Admin

Password: Admin

### sales.xlsx
Tab 1 : The Sales sheet containes a set of records with sales , values and profits.

Tab 2 : this is the output tab where you need to set the new values.

# CRM RPA Assignment

the goal from this assingment is to have a sheet with payment records matching the CRM on the output tab of the same sheet.

- Start from the Sales sheet where values might be not matching the records on the CRM portal.
- you need to calculate the profit after checking the amount
- the account id is you field to use in the search field
- you need to use the output tab (Tab 2).
- you need to read the first tab record by record and find it on the CRM

before you add any record to the sheet you need to check if the account is BlackListed using the BlackList Service

### BlackList Service

URL (GET): https://avertra-academy.herokuapp.com/card/check?id=<ACCOUNT_ID>

#### Not Blacklisted
```
{
    "result": false
}
```

#### Blacklisted
```
{
    "result": true
}
```



