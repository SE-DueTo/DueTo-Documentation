# Use-Case Specification: Add Transaction

# 1 Add Transaction

## 1.1 Brief Description
Every registered user is able to add a new transaction in order to request a payment. In this process the user can choose the preferred date for the payment and the ways (total amount, percentage, installments) and methods of the payment. Furthermore, the user can enter a creditor to whom the debt is owned. The user will be able to choose how the debt is distributed among the group members.The steps that the user can take are summarized below.

# 2 Flow of Events
## 2.1 Basic Flow
- User clicks the "Add a transaction" button
- User chooses the date on which the debts should be settled
- User adds an amount for the debt
- User can add an intended use
- User can be a creditor or can add a creditor
- User adds a payment method
- User chooses if the debt should be distributed equally
    - NO:
        - User chooses YES to add a percantage payment or NO to add an amount per member
        - User chooses YES for a repeated settling of a debt and adds an interval
        or chooses NO and goes straight to the "Send Transaction" button
    - YES: 
        - User chooses YES for a repeated settling of a debt and adds an intervall chooses NO and goes to the "Send Transaction" button
         

### 2.1.1 Activity Diagram
![Settle Debt Activity Diagram](https://drive.google.com/uc?id=1_uURahT5un0lH5y3K_RFsYyp9Z_TXIGJ)

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
After clicking the "Send" button the members of the group are notified about the requested transaction. 
 
# 6 Extension Points
(n/a)