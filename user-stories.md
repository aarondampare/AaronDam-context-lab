# User Stories — Account Management Context

## Story 1
As a bank customer
I want to open a new savings account online
So that I can start banking without visiting a branch

```gherkin
Scenario: Customer opens a new savings account
  Given the customer is on the registration page and provides a national ID, proof of address, and other required documents
  When the customer submits the application
  Then the system should validate the information provided
  And the system should create a new account
  And display the customer's account number and details to the customer
```

## Story 2
As a bank customer
I want to view my real-time account balance
So that I can make informed spending decisions before a payment fails

```gherkin
Scenario: Customer checks account balance after a recent transaction
  Given a customer has an account with a balance of "GHS 3200.00"
  When the customer requests to view their account balance
  Then the system should display the current balance of "GHS 3200.00"
  And show the timestamp of the last transaction
  And confirm the balance reflects all completed transactions in real time
```
