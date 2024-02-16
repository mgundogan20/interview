# UI Doc of the Admin View for User Management
The document here describes the User Management screen which allows site admins to add and view user accounts. 
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
6) Enabled:       A checkbox to choose whether the user will be created as an active account or not.
## Page Behaviour
### Initialization
The the existing users should be fetched from the database and be displayed in the "user list table". The fields of the "add user form" should be empty.
### Header
This division includes some buttons to let the admin manage the database and the page.
1) New User button should reset the add user form.
2) Hide Disabled User switch should change the visibility of accounts in the "User List Table" below.
3) Save User button should finalize the user registration process and save the user to the database if all the inputs are valid. When this is not case the user should be warned appropriately. This button should not submit the form twice.
### User List Table
This table shoudl list the existing accounts with every row containing a single account, columns of which display said account's data. When a new user is added, the table should be updated.
### Add User Form
This form should handle user registration. Each of its inputs should be validated. And the user should be warned in cases that the inputs are not valid.
1) Username:      Shouldn't include unpermitted characters, should be unique.
2) Display Name:  Shouldn't include unpermitted characters.
3) Phone:         Should be a valid, international phone number.
4) Email:         Should follow the email formatting standards.
5) User Roles:    One and only one role must have been selected.
## Requirements
### User Friendliness
All inputs should have proper labels and error messages to be shown when they couldn't be validated.
### Security
All form inputs should be checked and properly handled against injection attacks.
### Error Handling
All server-side errors should be caught and handled.

