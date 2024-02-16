# UI Doc for the Admin View for User Management
The document here describes the User Management screen which allows site admins to add and view user accounts. 
## Requirements

## UI components
### Header
This division includes some buttons to let the admin manage the database and the page.
1) New User:           A button to reset the form below to allow a new user to be registered.
2) Hide Disabled User: A toggle switch to choose the visibility of non active accounts in the "User List Table" below.
3) Save User:          A button to save a new user to the database according to the inputs of the "Add User Form" below.
### User List Table
This table lists the existing accounts in the system. Has the following collumns:
1) ID:        An auto incremented integer for each account.
3) User Name: User Name chosen by the user 
4) Email:     Their email address
5) Enabled:   A bool value to show whether the account is active or not.

### Add User Form
This constitutes the interface to add new users to the system, when the "Save User" button in the header is used, a new row in the user database is created according to the inputs from this form.
1) Username:      A text field input to get the new user's name.
2) Display Name:  A text field input to get the name which will be seen by other users.
3) Phone:         A tel field input to get the new user's telephone number.
4) Email:         An email field input to get a valid email for the new user.
5) User Roles:    A dropdown menu to choose from a set of roles, (guest, admin, super-admin).

## Page Behaviour

## What to Show to the User
