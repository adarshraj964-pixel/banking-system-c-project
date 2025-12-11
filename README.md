-----------------------------------------------------
   BANKING SYSTEM IN C (ATM + BINARY FILE HANDLING)
   Author: Adarsh Raj
   AP25110010009
------------------------------------------------------
   PROJECT TITLE
   ===================== 
BANKING SYSTEM IN C (ATM + BINARY FILE HANDLING)
 ---------------------
   PROJECT OVERVIEW
---------------------- 
This mini–project is a complete Banking Management System written in C.
It stores all account information using Binary Files (bank.dat).

The system includes:
- Account Creation
- Secure ATM Login (Account No + PIN)
- PIN Verification before withdrawal
- Deposit Money
- Withdraw Money
- Check Balance
- Change PIN
- Admin Panel (Protected with Admin PIN = 9999)

Binary files ensure data is permanent and secure.

 =====================
   FEATURES
 ===================== 

/* --- USER / ATM FEATURES --- */
1. Create Account
   - User enters Account Number, Name, PIN
   - Balance starts from 0
   - Data stored in bank.dat

2. ATM Login
   - Requires Account Number + PIN

3. Check Balance
   - Displays current account balance

4. Deposit Money
   - Adds amount
   - Updates binary file

5. Withdraw Money
   - Requires PIN again (security)
   - Checks sufficient balance
   - Updates file

6. Change PIN
   - User can update their ATM PIN

/* --- ADMIN FEATURES --- */
Admin PIN = 9999

Admin can:
- View all accounts (acc_no, name, pin, balance)
- This is PIN protected

/* =====================
   TECHNOLOGY USED
   ===================== */
Language     : C  
Compiler     : GCC / MinGW / Turbo C  
Storage File : bank.dat (Binary File)  
OS Support   : Windows / Linux / Mac  

=====================
   PROGRAM WORKING
 ===================== 

 --- STRUCTURE USED ---
struct Account {
    int acc_no;
    char name[50];
    int pin;
    float balance;
};

 --- FILE OPERATIONS USED --- 
fwrite() → Write account data  
fread()  → Read account data  
fseek()  → Move inside binary file  
ftell()  → Get position in file  

File Modes:
- ab  → Append new account
- rb  → Read accounts
- rb+ → Read + Update account

/* =====================
   PROJECT FILE STRUCTURE
   ===================== */
BankingSystemProject/
│
├── banking_system.c
├── bank.dat      (auto created on program run)
├── README.md
│
└── screenshots/

 =====================
   HOW TO COMPILE & RUN
  ===================== 

/* Windows */
gcc banking_system.c -o bank
bank.exe

/* Linux / macOS */
gcc banking_system.c -o bank
./bank

=====================
    SCREENSHOTS
==================== 
- Home.png
- Admin_login.png
- Atm_login.png
- Deposit_withdrawal.png
- Pin_change.png
- create_account.png
- Pin_change.png

Go to /screenshots folder to see screenshots

=====================
 FUTURE IMPROVEMENTS
===================== 
- PIN hidden input (****)
- Delete account feature
- Money transfer between accounts
- Transaction history
- Mobile No + OTP
- GUI version (Python/Java)
- Encrypted PIN storage
-------------------------

🔐 Admin PIN
To view all account records:
Admin PIN = 9999

📌 Important Notes
Make sure bank.dat is in the same directory as the exe/program.
Do not open bank.dat manually; it is a binary file.
The program automatically creates the file if not found.


📜 License
This project is created for educational purposes, academic submission, and basic demonstration of file-handling concepts in C.

-------------------------
   END OF README
--------------------------
