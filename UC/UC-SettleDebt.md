# Use-Case Specification: Settle Debt

# 1 Settle debt

## 1.1 Brief Description
Every registered user can settle an already existing debt. In this process the user can choose the preferred date for the payment and the ways (total amount, percentage, installments) and methods of the payment.  The steps that the user can take are summarized below.

# 2 Flow of Events
## 2.1 Basic Flow
- User clicks the "Settle debts" button
- User chooses the date on which the debts should be settled
- User adds a "Creditor"
- User can choose:
    - YES: for a payment of the total amount
        - User adds a payment method
        - User clicks the "Send" button
    - NO: for an installment plan
        - User chooses YES to add a percantage payment or NO to add an amount
        - User chooses YES for a repeated settling of a debt and adds an interval
        - User adds a payment method
        - User clicks on the "Send" button
         

### 2.1.1 Activity Diagram
![Settle Debt Activity Diagram](https://drive.google.com/uc?id=1OZ6hb4l8F73X_CataX6k-0ZrXDKe_JKk)

### 2.1.2 Mock-up
![Settle Debt Form Wireframe]()

### 2.1.3 Narrative
tbd

## 2.2 Alternative Flows
(n/a)

# 3 Special Requirements
(n/a)

# 4 Preconditions
## 4.1 Login
The user has to be logged in in the system.

# 5 Postconditions
After clicking the "Send" button the Creditor is notified about the payment. 
 
# 6 Extension Points
(n/a)