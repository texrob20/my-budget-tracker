# PWA Challenge
GIVEN a budget tracker without an internet connection:

- WHEN the user inputs an expense or deposit THEN they will receive a notification that they have added an expense or deposit
- WHEN the user reestablishes an internet connection THEN the deposits or expenses added while they were offline are added to their transaction history and their totals are updated

## Created With:
- Node js
    - Express
    - Mongoose
- MongoDB
- HTML
  - IndexedDB
  - Service Workers
  - Cache
- CSS  
- Heroku

## Budget Tracker Application
This application allows user to deposit or debit transactions in their budget tracker.

### Online Functionality
When online the application connects to a MongoDB to store the transactions in a database.  As each transaction is added or subtracted the transaction database and total are updated.

### Offline Functionality
When the application is offline, a service worker, cache, and IndexedDB are used to store the transactions until the application is back online.  Once the application is online again, the service worker will update the backend database.

## Deployed App
The application can be tested here: https://safe-everglades-18834.herokuapp.com/

## Demo

<img src=https://github.com/texrob20/my-budget-tracker/blob/main/demo/my-budget-demo.png>