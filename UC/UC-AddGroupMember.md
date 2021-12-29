# Use-Case Specification: Settle Debt

# 1 Settle debt

## 1.1 Brief Description
Every registered user can settle an already existing debt. In this process the user can choose the preferred date for the payment and the ways (total amount, percentage, installments) and methods of the payment.  The steps that the user can take are summarized below.

# 2 Flow of Events
## 2.1 Basic Flow
- User clicks on the "GroupDashboard" Button
- User clicks on the "addGroupMember" Button
- User insert the "Username" in Textfield
- if "Username" exist:
    - NO: 
        - User insert new "Username"
    - YES:
        - User clicks on the "addToGroup" Button
         

### 2.1.1 Activity Diagram
![Settle Debt Activity Diagram](https://drive.google.com/file/d/16Un_5Ptxm9VFc0MCEsA_WhYm_8Hy6k_3/view?usp=sharing)

### 2.1.2 Mock-up
(n/a)

### 2.1.3 Narrative
(n/a)

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