QuickChat - Registration and Login System

📌 Project Overview

QuickChat is a simple Java console application developed as part of the PROG5121 Part 1 POE. The system allows a user to register an account and then log in using the registered credentials.

The application demonstrates the use of object-oriented programming concepts, input/output handling, validation, and decision-making structures.

⚙️ Features
	•	User registration with:
	•	Username validation
	•	Password complexity validation
	•	South African cellphone number validation
	•	Login functionality
	•	User authentication feedback messages
	•	Unit testing using JUnit


🧠 Validation Rules

Username
	•	Must contain an underscore (_)
	•	Must not be more than 5 characters long

Password
	•	Must be at least 8 characters long
	•	Must contain:
	•	A capital letter
	•	A number
	•	A special character

Cellphone Number
	•	Must start with +27 (South African international code)
	•	Must be 12 characters long
	•	Must contain only numeric digits after +27


🏗️ Project Structure

1. QuickChat Class

Handles:
	•	User input (registration and login)
	•	Calls methods from the Login class
	•	Displays output messages

2. Login Class

Contains all system logic:
	•	Username validation
	•	Password validation
	•	Cellphone validation
	•	User registration
	•	Login verification
	•	Login status messaging

3. User Class

Stores user information:
	•	First name
	•	Last name
	•	Username
	•	Password
	•	Cellphone number

4. TestUnit Class

Contains JUnit tests to verify:
	•	Username validation
	•	Password validation
	•	Cellphone validation
	•	Registration functionality
	•	Login functionality


🧪 Testing

JUnit is used to test system functionality. The following tests are included:
	•	Username validation (valid and invalid)
	•	Password complexity (valid and invalid)
	•	Cellphone format (valid and invalid)
	•	Login success and failure
	•	Login status messages

🚀 How to Run the Program
	1.	Open the project in NetBeans
	2.	Run the QuickChat class
	3.	Enter user details when prompted
	4.	Register and then log in using the same credentials

🔧 Technologies Used
	•	Java
	•	NetBeans IDE
	•	JUnit (for testing)
	•	Maven (project management)
