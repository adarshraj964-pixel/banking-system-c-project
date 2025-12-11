# banking-system-c-project
Simple Banking System in C using Binary File Handling and ATM features.
# banking-system-c-project
Simple Banking System in C using Binary File Handling and ATM features.

Bank Management System (C Program)

This project is a simple Bank Management System implemented in the C programming language.
It allows users to create bank accounts, log in through an ATM interface, and perform various banking operations such as balance inquiry, deposit, withdrawal (with PIN verification), and PIN change.
An additional admin section allows authorized personnel to view all stored accounts.

📌 Features
1. Create New Account
Stores a new customer's account number, name, PIN, and starting balance (0 by default).
Saves data in a binary file (bank.dat).

2. ATM Login
Users log in using Account Number + PIN.
After successful authentication, they can:
Check balance
Deposit money
Withdraw money (with PIN verification)
Change PIN
Logout

3. Admin Access

Shows all account records.
Protected by Admin PIN: 9999.

4. Data Storage

Accounts are stored using structures in a binary file.
Uses fread() and fwrite() for safe reading and writing.

📁 Project Structure

Bank-Management-System/
│
├── main.c          # Complete C source code
├── bank.dat        # Auto-generated after running the program
├── README.md       # Project documentation
└── screenshots/    # Screenshots of output (add your images here)

🛠 Technologies Used
C Programming
File Handling (Binary Files)
Structures in C
ATM-Style Menu System

📸 Screenshots
Create a folder named screenshots/ and add images such as:
Program start screen
Create account
ATM login
Deposit / Withdraw
Admin display

Example filenames:

screenshots/home_menu.png
screenshots/create_account.png
screenshots/atm_login.png
screenshots/withdraw_pin_verification.png

▶ How to Run
Using GCC
gcc main.c -o bank
./bank

On Windows (MinGW)
gcc main.c -o bank.exe
bank.exe

🔐 Admin PIN
To view all account records:
Admin PIN = 9999

📌 Important Notes
Make sure bank.dat is in the same directory as the exe/program.
Do not open bank.dat manually; it is a binary file.
The program automatically creates the file if not found.


📜 License
This project is created for educational purposes, academic submission, and basic demonstration of file-handling concepts in C.
