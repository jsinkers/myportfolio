# myportfolio

Django-based web-app to keep track of your share portfolio and other market
data.

## Model Requirements

### Security data
Should represent open/high/low/close/volume data at a given time for a given 
security, on a given exchange, with a given currency.  This should be generic 
so it could represent shares on the ASX or cryptocurrency.

There should be a way to handle:
- stock splits
- mergers
- changes to company name/symbol
- dividends 

### Trade data
Should represent a buy/sell, and capture any fees.

### Deposits/withdrawals
Users should be able to deposit/withdraw cash

### Accounts
Should contain securities and cash. 

Later feature:
- support for margin loans, LVR, etc.

## View Requirements

### Security view
View a chart for a given security.  

- Candlestick preferred, with option for line.
- Comparison to other securities?
- Technical analysis

### Portfolio view
View chart and table of accounts with corresponding market value for timeline

- Rate of return, time-weighted
- Rate of return, money-weighted
- Add account

### Account view
View chart and table of account securities + cash, with corresponding market value
selectable by date range

- Portfolio breakdown by % security
- Rate of return as per portfolio view

### Transaction view
View transactions on a given account.  

- Add transactions

### Email
Get periodic summary of performance, dividends, etc.
 
## Controller Requirements
 
### Data update
Periodic download of data from specified data source and importing to the database.

### Transaction update
Users should be able to import csv files with specified format for transactions



 
