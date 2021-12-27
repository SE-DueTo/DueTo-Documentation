# Use-Case Specification: Create a Group

## 1. CRUD: Create a group

### 1.1 Brief Description

This use case describes the creation, reading, updating and deleting of Groups (CRUD).

## 2. Flow of Events

![CRUD Groups](https://drive.google.com/uc?id=14t7JpXWMp73SGgkAIXUaw5l-OX3LMwKn)

### 2.1 Basic flow
Generally, the user can create and list all of his groups. It is also possible to edit the groups by adding and removing members. Furthermore, the user will be able to delete a group.

### 2.2 Creation  

By creating a new group the user will be asked to enter a name and a text.

### 2.3 Edit

During editing the user can modify the name and add or remove members of the group.


### 2.3 List

The user will to be able to view all of his groups. Here, he is presented a list with all entries.


### 2.4 Delete

The user will be able to delete existing groups. Therefore, we added a button for the deletion of the group. To ensure he does not delete a group on accident we added a modal asking if he really wants to do this.


## 3. Special Requirements

### 3.1 Owning An Account
        
In order to create a new group the user has to have an account. Only if he has one, the dialog of a creation of a group will be visible.

## 4. Preconditions

### 4.1 The user has to be logged in

To ensure proper privacy of the groups the user has to be logged in when editing/creating a group.

## 5. Postconditions

### 5.1 Create

After creating the new group the user will be redirected to the list overview, where the new entry will be displayed.

### 5.2 Edit

After the user saves his edits, the updated data will be displayed in the list overview.

### 5.3 Delete

After confirming the deletion modal, the group will be permanently removed and no longer displayed in the list overview.

## 6. Function Points
tbd