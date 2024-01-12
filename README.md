# Password-Manager
Background:
Password security is an essential component of cybersecurity. Safeguarding user passwords is critical in
many applications, including personal accounts and enterprise systems, to protect sensitive information.
The goal of this project is to develop a password manager that not only securely stores passwords but also
encrypts them with a key, thereby increasing the security of saved credentials.
Objectives:
The following are the main objectives of the password manager:
a) Create a password manager that saves and encrypts user credentials securely.
b) Use strong encryption mechanisms to safeguard passwords.
c) Include features for adding, retrieving, and modifying passwords.
d) Implement a secure and user-friendly command-line interface (CLI) for interaction.
Scope:
The project is to develop a password manager that securely stores and encrypts the password given by
the user. It uses a command line interface (CLI) to take inputs like adding a new user and passwords and
retrieve and update passwords. The passwords are stored in a text file with encryption applied for added
security.
Implementation:
The key features of the password manager include:
a) SHA-256 hashing and bitwise XOR encryption are used for password encryption.
b) New usernames can be added and updated.
c) Retrieval of previously saved passwords for a specified username.
d) Replacing old passwords with new ones.
e) Safely save passwords in a text file.
f) For each session, a random encryption key is generated.
Components:
The main components of the application are as follows:
a) Encryption functions: These functions handle encryption and decrypt techniques using
cryptographic techniques.
b) Password Management functions: These allow users to create, retrieve, and update passwords.
c) Main Application Logic: A command line is included so that the user can provide an input through
it.
Scope:
a) The goal of this project is to create a password management application that uses password
encryption to increase security.
b) Users can add, retrieve, and update passwords via the application's command-line interface (CLI).
c) For further security, the passwords are stored in a text file that has been encrypted.
Implementation:
The key features of the password manager with encryption include:
a) SHA-256 hashing and bitwise XOR encryption are used for password encryption.
b) Adding new passwords as well as usernames.
c) Retrieve cached passwords for a specified username.
d) Replacing old passwords with new ones.
e) Secure storage of passwords in a text file.
f) For each session, a random encryption key is generated.
Components:
The main components of the application are as follows:
Libraries used:
Os library: This library is used to interact with different os systems allowing us to perform file handling
functions and directory operation.
Hashlib library: This library provides a secure way to generate hash values for data like strings, files or
binary data.
Encryption functions: These functions handle password encryption and decryption using cryptographic
techniques.
SHA256 (secure hashing algorithm) is a hash function which is a mathematical algorithm that takes an
input and returns a string of fixed size in bytes. The output is 256 bits long, or 32 bytes or 64 hexadecimal
characters. In this program, we take the input in bytes using UTF-8 encoding and then we convert the
hashed value into a hexadecimal value.
In summary, this code accepts a password as input, transforms it into bytes, hashes those bytes using the
SHA-256 algorithm, and outputs the hash as a hexadecimal string. Because it transforms the password into
a fixed-length string of characters that cannot be easily reversed to disclose the original password, hashing
is a popular method for securely storing passwords.
Password management functions:
a) Add function: In this function, the encrypted password is encoded in bytes. This encrypted
password is then passed in the file in binary append mode. The passwords for all the users will be
saved in this file.
b) Retrieve function: Given a user's username and an encryption key, this function can retrieve the
user's decrypted password from the file. We have created a load_password function which
retrieves the password from the file. The password is then decrypted and returned to the user.
c) Update function: After checking if the username exists in the file, the new password is encoded
and replaces the old password. The new updated password is returned to the user.
d) Main Application Logic: The main application logic provides a command-line interface (CLI) for
user interaction. The user can select if they want to add, retrieve or update the password.
