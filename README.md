# POEpt1
Overview
This Java application implements a user registration and login system as required for the PROG5121 Practical Examination (PoE). The system validates usernames, passwords, and South African cell phone numbers according to specific complexity rules.

Features
User Registration:

Username validation (must contain underscore and be ≤ 5 characters)

Password complexity validation (8+ characters, capital letter, number, special character)

South African cell phone validation with international code

User Login:

Credential verification against stored registration data

Personalized welcome messages for successful logins

Input Validation:

Comprehensive validation with appropriate error messages

Regular expression-based phone number validation

Requirements
Java JDK 8 or higher

JUnit 5 (for testing)

Implementation Details
Main Classes
RegistrationLoginSystem: Main class that handles user interaction

Login: Core class containing all validation and authentication logic

Key Methods
checkUserName(): Validates username format

checkPasswordComplexity(): Ensures password meets complexity requirements

checkCellPhoneNumber(): Validates SA cell phone format using regex

registerUser(): Handles the complete registration process

loginUser(): Authenticates user credentials

returnLoginStatus(): Generates appropriate login status messages

Validation Rules
Username:

Must contain an underscore (_)

Maximum 5 characters long

Password:

At least 8 characters long

Contains at least one capital letter

Contains at least one number

Contains at least one special character

Cell Phone:

Must include international country code (+27 or 027)

Must be followed by 9 digits

Example valid format: +27838968976

AI Usage Attribution
The regular expression for South African phone number validation was created with assistance from ChatGPT:

Reference: OpenAI. (2023). ChatGPT (Mar 14 version) [Large language model]. https://chat.openai.com/chat

Unit Testing
Comprehensive JUnit tests are provided to verify all functionality:

Username validation (correct and incorrect formats)

Password complexity checking

Cell phone number validation

Registration process

Login functionality

Status message generation

To run tests: Execute the LoginTest class with JUnit 5

Usage

Compile the Java files:

javac RegistrationLoginSystem.java


Run the application:

java RegistrationLoginSystem

Follow the prompts to register and then login

Good Coding Practices
This implementation demonstrates:

Object-oriented programming principles

Separation of concerns

Input validation and error handling

Test-driven development approach

Clean, maintainable code structure

Proper attribution of AI-assisted code

Academic Integrity
This solution is individual work created in accordance with PROG5121 POE requirements. All external resources including AI assistance have been properly referenced following APA guidelines.
