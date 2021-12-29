# Use-Case Specification: Settle Debt

# 1 Settle debt

## 1.1 Brief Description
Any registered user can create a new group. To do this, he must specify a group name, as well as add other users to the group. The required steps are described in more detail below.

# 2 Flow of Events
## 2.1 Basic Flow
- User clicks on the "addGroup" button
- User inser "Groupname" in textfield
- User clicks on the "create" button
- User insert the "Username" in textfield
- if "Username" exist:
    - NO: 
        - User insert new "Username"
    - YES:
        - User clicks on the "addToGroup" Button
            - User insert new "Username"
            - User clicks on the "create" Button
         

### 2.1.1 Activity Diagram
![Add Group Activity Diagram](https://drive.google.com/file/d/10lm4-NJgDR2PmNlnbZXSYM-EfX2g6jlr/view?usp=sharing)

### 2.1.2 Mock-up
![Insert Groupname Form Wireframe](https://drive.google.com/file/d/1EWdGvw8p50oudS2X-YbY4Yr1AV0rk7Rq/view?usp=sharing)
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