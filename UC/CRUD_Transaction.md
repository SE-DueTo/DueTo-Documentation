# Use-Case Specification: Transactions

## 1. CRUD: Transactions

### 1.1 Brief Description

This use case describes the creation, reading, updating and deleting of transactions (CRUD).

## 2. Flow of Events

![CRUD Transaction](https://drive.google.com/uc?id=1hPavCfXMP0aJiT814f-xc29NtRdmUARr)

### 2.1 Basic flow
Generally, the user can create and list all of his transactions. It is also possible to edit the transactions. Furthermore, the user will be able to delete his transactions.

### 2.2 Creation  

The user will be able to create new transactions with a name, reason for the transaction and the amount.

### 2.3 Edit

During editing the user can modify the transactions: change the name of the transaction, change the amount and the reason for the transaction.

### 2.3 List

The user will to be able to view all of his transactions, where he is presented a list with all his entries.

### 2.4 Delete

The user will be able to delete existing transactions.

## 3. Special Requirements

### 3.1 Owning An Account
        
In order to create a new transaction the user has to have an account. Only if he has one, the dialog of a creation of a new transaction will be visible.

## 4. Preconditions

### 4.1 The user has to be logged in

To ensure proper privacy of the transactions the user has to be logged in when editing/creating a transaction.

## 5. Postconditions

### 5.1 Create

After creating the new transaction the user will be redirected to the list overview, where the new entry will be displayed.

### 5.2 Edit

After the user saves his edits, the updated data will be displayed in the list overview.

### 5.3 Delete

After deletion the transaction will be permanently removed and no longer displayed in the list overview.

## 6. Function Points
tbd