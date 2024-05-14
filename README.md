# Signup System in PHP with MySQL Database

## Description
This PHP script provides a simple signup system with error handling for checking input fields, email validity, and username/email availability in a MySQL database.

## Requirements
- PHP
- MySQL

## Setup
1. Create a MySQL database with a table named `users` containing columns for `username`, `pwd` (password), and `email`.
2. Update the database connection settings in `config.php` with your MySQL database credentials.
3. Upload the files to your server.

## Error Handlers
The script uses the following error handlers:

### is_input_empty($username, $pwd, $email)
Checks if any of the input fields (username, password, email) are empty.

### is_email_invalid($email)
Checks if the email format is invalid.

### is_username_taken($pdo, $username)
Checks if the username is already taken in the database.

### is_email_registered($pdo, $email)
Checks if the email is already registered in the database.

If any of these conditions are met, the corresponding error message is displayed to the user.

## Usage
1. Access the signup form (`signup.php`) through your web browser.
2. Fill in the required fields (username, password, email) and submit the form.
3. If there are any errors, they will be displayed on the signup form.
4. If there are no errors, the user will be added to the database.

## Disclaimer
This is a basic signup system for educational purposes. It is not intended for production use without further security enhancements.
