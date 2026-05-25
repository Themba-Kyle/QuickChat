# QuickChat Application

## Overview
QuickChat is a Java console-based messaging application that allows users to:

- Register a new account
- Log in securely
- Send messages
- Store messages for later
- Validate phone numbers
- Validate message length
- Generate unique message IDs
- Create message hashes
- Count total sent messages

The application simulates a basic chat system with user authentication and messaging functionality.

---

## Features

### User Registration
Users must provide:

- First name
- Last name
- Username
- Password
- Cellphone number

Validation includes:

#### Username Requirements
- Must contain an underscore (`_`)
- Must not exceed 5 characters

Example:

john_

---

#### Password Requirements
Password must contain:

- At least 8 characters
- At least 1 uppercase letter
- At least 1 number
- At least 1 special character

Example:

Password1!

---

#### Cellphone Requirements
Phone numbers must:

- Start with `+27`
- Be exactly 12 characters long
- Contain only digits after `+27`

Example:

+27831234567

---

## Login System

After registration, users can log in using:

- Username
- Password

Features:

- Maximum of 3 login attempts
- Displays a welcome message after successful login
- Exits program after 3 failed attempts

---

## Messaging Features

After login, users can access the QuickChat menu.

### Send Messages
Users can:

- Enter recipient phone number
- Enter message text
- Send message
- Store message for later
- Delete message

---

### Message Validation

#### Message Length Check
Messages must not exceed **250 characters**.

If exceeded, the program shows:

```text
Message exceeds 250 characters by X; please reduce the size.
```

---

#### Recipient Validation
Recipient numbers must:

- Start with `+27`
- Be exactly 12 characters
- Contain only numbers after country code

---

## Message ID Generation

Each message is assigned a randomly generated **10-digit unique ID**.

Example:

```text
1234567890
```

---

## Message Hash Creation

A message hash is generated using:

- First two digits of Message ID
- Message number
- First word of the message
- Last word of the message

Format:

```text
ID:MessageNumber:FIRSTWORDLASTWORD
```

Example:

```text
12:1:HELLOWORLD
```

---

## Store Messages

Messages can be saved into a local JSON file:

```text
messages.json
```

Stored information includes:

- Message ID
- Message Number
- Recipient
- Message Text
- Message Hash

Example JSON:

```json
{
  "messageID": "1234567890",
  "messageNumber": 1,
  "recipient": "+27831234567",
  "messageText": "Hello there",
  "messageHash": "12:1:HELLOTHERE"
}
```

---

## Total Messages Counter

The application keeps track of successfully sent messages.

Example output:

```text
Total messages successfully sent: 3
```

---

## Project Structure

```text
QuickChat/
│
├── QuickChat.java     # Main application and menu
├── Login.java         # Registration and login validation
├── Message.java       # Message handling and storage
├── User.java          # User data model
└── messages.json      # Stored messages
```

---

## Technologies Used

- Java
- NetBeans IDE
- Object-Oriented Programming (OOP)
- File Handling (JSON storage)
- Scanner for user input
- Random class for ID generation

---

## How to Run

### Step 1
Open the project in **NetBeans IDE**.

### Step 2
Run:

```text
QuickChat.java
```

### Step 3
Follow prompts:

1. Register account
2. Login
3. Choose messaging options

---

## Example Program Flow

```text
Enter first name:
Kyle

Enter last name:
User

Enter username:
ky_le

Enter password:
Password1!

Enter cellphone:
+27831234567

Welcome Kyle User

=== LOGIN ===
Enter your username:
ky_le

Enter your password:
Password1!

Welcome Back Kyle User

=== QuickChat Menu ===
1. Send Messages
2. Show recently sent messages
3. Quit
```

---

## Future Improvements

Planned features include:

- Show recently sent messages
- Delete stored messages
- Search messages
- GUI version of QuickChat
- Database storage
- Encryption improvements

---

## Author

Kyle User

---

## License

This project is for educational purposes.
