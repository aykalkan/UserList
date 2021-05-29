# About UserList
UserList is a handy tool to manage see, manage and add users to your website. UserList turns tedious user management jobs into an enjoyable experience.

# UserList Structure
UserList consist of three main components.
* Top bar
* The users list
* New user form

## Top Bar
On the top bar there should be 3 elements.
* New user button
* Save user button
* Hide disabled user checkbox

#### New user button
This button will be used when a new user wanted to be added to the system. When someone presses that button "new user form" should be shown on the screen.

This button should be aligned to the left on the top bar. Button should be in primary colors and it should have a plus icon next to the button text.

#### Save user button
This button will be used after completing a new user form. It saves the data in the form to the database.

Button will be on right aligned in the screen and it should be in info colors.

#### Hide disabled user checkbox
This checkbox give opportunity to hide disabled users while listing users. Making a user enable/disable will be explained in new user form.

Checbox should be aligned left next to new user button.

## The Users List
Users list is landing page of the project. It shows all registered users (unless "Hide Disabled User" checkbox checked). Users are listed in four cloumns.

* ID
* User Name
* Email
* Enabled

All columns will be sortable and filterable.

## New User Form
When a new user wanted to be added this form will be used. There are 6 form elements in this form.

* Username
* Display name
* Phone
* Email
* User roles
* Enabled

All of the elements are required. So there should be input checki via Javascript before accepting the form. There should be also input integrity checks which varies element to element.

#### Username
This is a simple `text` input to receive the user's real name. This field must be at least 2 words and have only letters. These must be checked via Javascript. 
#### Display name
This field is a `text` input and a nickname input is expected. This field must be between 4-20 characters in any form and there should be uniqueness check at form sending.
#### Phone
This is a `tel` input type form element. It receives phone numbers in `+90 505 700 8454` pattern. Correctness checks should be done via Javascript.
#### Email
This is a `email` type form element. E-mail correctness should be checked and this field must be uniqe which be checked at form sending.
#### User roles
This field is a `select` form element. There are 3 user roles will be listed.
* Guest
* Admin
* SuperAdmin
There isn't any default user role will shown. There could be a "Select user roles..." message in the field.
#### Enabled
This is a `checkbox` form element. When not checked the new user will be recordad as disabled.
