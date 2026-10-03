# 📧 Python Email Simulator (OOP)

A command-line email simulation system built with **Python**, utilizing **Object-Oriented Programming (OOP)** principles. This application models real-world email interactions between different users, managing inboxes, message read states, and secure message handling.

---

## 🚀 Features

*   **User Management:** Create distinct users with their own independent mailboxes.
*   **Email Transmission:** Send emails seamlessly from one user to another with custom subjects and bodies.
*   **Inbox Organization:** List all received emails with real-time index tracking.
*   **Read / Unread Status:** Automatically track whether an email has been opened and read.
*   **Message Operations:** Read full message details with formatted timestamps or delete unwanted emails from the inbox.

---

## 📂 Project Structure

```text
├── email_system.py   # Contains Email, User, and Inbox classes along with main execution flow
└── README.md         # Project documentation


from email_system import User

# Create users
tory = User('Tory')
ramy = User('Ramy')        

# Send emails
tory.send_email(ramy, 'Hello', 'Hi Ramy, just saying hello!')
ramy.send_email(tory, 'Re: Hello', 'Hi Tory, hope you are fine.')

# Check inbox and read messages
ramy.check_inbox()
ramy.read_email(1)

# Delete message
ramy.delete_email(1)
ramy.check_inbox()
