# 📚 Library Management System

A simple **Library Management System** developed in **C** using **Structures, Arrays, Modular Programming, and File Handling**. This project provides a menu-driven interface to efficiently manage book records, issue and return books, and maintain library data. It demonstrates C programming, file operations, date handling, and modular programming using multiple source files.

---

## 📌 Features

- ➕ Add New Book
- 📋 Display All Books
- 🔍 Search Book by Book ID
- 🔍 Search Book by Book Name
- 🔍 Search Book by Author Name
- ✏️ Modify Book Details
- ❌ Delete Book Record
- 📖 Issue Book
- 🔄 Return Book
- 📑 List Issued Books
- 💾 Save Book Records
- 📂 Load Previously Saved Data
- 🆔 Automatically Generate Unique Book ID
- 📅 Automatically Generate Issue Date
- 📅 Automatically Calculate Due Date
- 📅 Automatically Record Return Date
- 💰 Calculate Fine for Late Returns
- 🚪 Save and Exit
- 🚪 Exit Without Saving

---

## 🛠️ Technologies & Tools Used

- C Programming
- GCC Compiler
- Linux
- Makefile
- Data Structures (Structures and Arrays)
- File Handling
- Date and Time Functions
- Modular Programming

---

## 📚 Concepts Used

- Structures
- Arrays
- Functions
- `extern` Variables
- Modular Programming
- Multiple Source Files
- File Handling
- String Handling
- Date and Time Functions
- Loops
- Conditional Statements
- `switch-case`
- GCC Compilation
- Makefile

---

## 📁 Project Structure

```text
LIBRARY-MANAGEMENT-SYSTEM-LMS/
├── library.c
├── add.c
├── remove.c
├── update.c
├── search.c
├── show.c
├── issue.c
├── return.c
├── list.c
├── save.c
├── load.c
├── exit.c
├── Makefile
├── books.txt
├── issues.txt
└── README.md

## Learning Outcomes

Through this project, I gained practical knowledge and hands-on experience in:

Implementing Structures and Arrays for library book management.
Performing CRUD operations such as Add, Display, Search, Update, and Delete.
Using File Handling functions such as fopen(), fclose(), fprintf(), and fscanf() for data storage and retrieval.
Implementing Issue and Return operations for library books.
Automatically generating unique Book IDs.
Automatically generating Issue Date and Due Date.
Calculating fine amounts for late book returns.
Using Structures to organize book and issue information.
Developing a menu-driven console application in C.
Organizing code using modular programming with multiple source files.
Using extern variables to share data between different C files.
Compiling and managing the project using GCC and Makefile.
Improving problem-solving, debugging, and programming skills in C.

## Project Workflow
                    Start
                      │
                      ▼
              Load Saved Data
                      │
                      ▼
             Display Main Menu
                      │
                      ▼
             User Selects Option
                      │
        ┌─────────────┼─────────────┐
        │             │             │
        ▼             ▼             ▼
    Add Book      Search / Show   Update / Delete
        │             │             │
        └─────────────┼─────────────┘
                      │
                      ▼
                Issue Book
                      │
                      ▼
                Return Book
                      │
                      ▼
              Calculate Fine
                      │
                      ▼
               Save Records
                      │
                      ▼
                Exit Program
                      │
                      ▼
                     End

##Workflow Steps

The program starts and loads previously saved library data.
The main menu is displayed.
The user selects an operation.
Book records are stored using structures and arrays.
The user can Add, Display, Search, Update, and Remove books.
The system automatically generates a unique Book ID when a new book is added.
A book can be issued to a user after checking its availability.
The system automatically records the Issue Date and Due Date.
When a book is returned, the system records the Return Date.
If the book is returned late, the system calculates the fine amount.
The available book quantity is updated during issue and return operations.
The Save option stores the book and issue records into files.
The user can choose Save and Exit, Exit Without Saving, or Cancel.
The program continues until the user selects the Exit option.
📸 Sample Output
Main Menu
+----------------------------------------+
|       LIBRARY MANAGEMENT SYSTEM        |
+----------------------------------------+
|  1. Add Book                           |
+----------------------------------------+
|  2. Remove Book                        |
+----------------------------------------+
|  3. Update Book                        |
+----------------------------------------+
|  4. Search Book                        |
+----------------------------------------+
|  5. Issue Book                         |
+----------------------------------------+
|  6. Return Book                        |
+----------------------------------------+
|  7. List Books                         |
+----------------------------------------+
|  8. Show Book                          |
+----------------------------------------+
|  9. Save Book                          |
+----------------------------------------+
| 10. Exit                               |
+----------------------------------------+

Enter your choice:
➕ Add Book
========================================
              ADD NEW BOOK
========================================

Generated Book ID: 1

Enter Book Name: C Programming
Enter Author Name: Dennis Ritchie
Enter Quantity: 5

Book added successfully!

Book Details
-------------------------
Book ID  : 1
Title    : C Programming
Author   : Dennis Ritchie
Quantity : 5
-------------------------
📋 Display All Books
+--------------------------------------------------------------------------------+
|                              ALL BOOKS                                         |
+--------------------------------------------------------------------------------+
| Book ID  | Title                     | Author                    | Quantity |
+----------+---------------------------+---------------------------+----------+
| 1        | C Programming             | Dennis Ritchie            | 5        |
+----------+---------------------------+---------------------------+----------+
| 2        | Embedded C                | Michael J. Pont           | 3        |
+----------+---------------------------+---------------------------+----------+
| 3        | Linux                     | Linus                     | 4        |
+----------+---------------------------+---------------------------+----------+

Total Books: 3
🔍 Search Book
========================================
              SEARCH BOOK
========================================

A. By Book ID
B. By Book Name
C. By Author Name
D. Back to Main Menu

Enter your choice: A

Enter Book ID: 1

Book Found!

Book Details
-------------------------
Book ID  : 1
Title    : C Programming
Author   : Dennis Ritchie
Quantity : 5
-------------------------
✏️ Update Book
========================================
          UPDATE BOOK DETAILS
========================================

A. By Book ID
B. By Book Name
C. Back to Main Menu

Enter your choice: A

Enter Book ID: 1

What do you want to update?

1. Book Name
2. Author Name
3. Quantity
4. Cancel

Enter your choice: 3

Enter New Quantity: 10

Quantity updated successfully!
❌ Remove Book
========================================
             REMOVE BOOK
========================================

A. By Book ID
B. By Book Name
C. Back to Main Menu

Enter your choice: A

Enter Book ID: 2

Book removed successfully!
📖 Issue Book
========================================
              ISSUE BOOK
========================================

Enter Book ID: 1

Enter User ID: 101
Enter User Name: Poomalar

========================================
          BOOK ISSUED SUCCESSFULLY
========================================

Issue ID   : 1
Book ID    : 1
User ID    : 101
User Name  : Poomalar
Issue Date : 13-08-2026
Due Date   : 20-08-2026
========================================
🔄 Return Book
========================================
              RETURN BOOK
========================================

Enter Book ID: 1
Enter User ID: 101

Book returned successfully.

Return Date : 20-08-2026
Fine Amount : Rs.0
📑 List Issued Books
+------------------------------------------------------------------------------------------------+
|                                      ISSUED BOOKS                                              |
+----------+----------------------+----------+----------------------+------------+------------+
| Book ID  | Book Title           | User ID  | User Name            | Issue Date | Due Date   |
+----------+----------------------+----------+----------------------+------------+------------+
| 1        | C Programming        | 101      | Poomalar             | 13-08-2026 | 20-08-2026 |
+----------+----------------------+----------+----------------------+------------+------------+
💾 Save Records
========================================
                SAVE
========================================

Book records saved successfully.
Issue records saved successfully.
📂 Load Records
========================================
                LOAD
========================================

Book records loaded successfully.
Issue records loaded successfully.
🚪 Exit
========================================
                 EXIT
========================================

A. Save and Exit
B. Exit Without Save
C. Cancel

Enter your choice: A

Data saved successfully!
Program exiting...
🆔 Automatic Book ID Generation

The system automatically generates a unique Book ID.

For example, if the existing Book IDs are:

1
3
4

When a new book is added:

Generated Book ID: 2

The system finds the smallest available ID instead of asking the user to enter the ID manually.

Example:

Existing IDs:

1
3
4

New Book
   ↓
Generated ID = 2
📖 Book Issue and Return System

When a book is issued, the system records:

- Issue ID
- Book ID
- User ID
- User Name
- Issue Date
- Due Date
- Return Date
- Fine Amount
- Return Status

The available book quantity is reduced when a book is issued.

When the book is returned, the available quantity is increased.

💰 Fine Calculation

A fine is calculated when a book is returned after the due date.

Fine Amount = Number of Late Days × ₹5

Example:

Late Days = 3

Fine = 3 × ₹5

Fine = ₹15
💾 File Handling

The project uses File Handling to store library data permanently.

Book File
books.txt

Stores:

Book ID
Book Title
Author Name
Quantity
Issue File
issues.txt

Stores:

Issue ID
Book ID
User ID
User Name
Issue Date
Due Date
Return Date
Fine Amount
Return Status

This allows previously saved data to be loaded when the program starts again.

⚙️ Compilation
Using Makefile
make
Or Compile Manually
gcc library.c exit.c show.c list.c save.c return.c issue.c add.c update.c remove.c search.c -o lms
▶️ Run the Program
./lms
🧹 Clean Build
make clean
🧠 Project Highlights

This project is divided into multiple C source files. Each file is responsible for a specific library operation.

                     library.c
                         │
        ┌────────────────┼────────────────┐
        │                │                │
        ▼                ▼                ▼
      add.c          update.c         remove.c
        │                │                │
        └────────────────┼────────────────┘
                         │
        ┌────────────────┼────────────────┐
        │                │                │
        ▼                ▼                ▼
    search.c          show.c           list.c
        │                │                │
        └────────────────┼────────────────┘
                         │
        ┌────────────────┼────────────────┐
        │                │                │
        ▼                ▼                ▼
     issue.c          return.c          save.c
                         │
                         ▼
                      exit.c

Modular programming makes the project easier to:

Understand
Debug
Maintain
Modify
Extend
🔮 Future Improvements

Possible future enhancements:

🔐 Admin Login System
👥 User Management
📊 Library Reports
📈 Most Issued Books Report
⏰ Overdue Books Report
💰 Total Fine Collection Report
🔎 Case-Insensitive Search
🛡️ Advanced Input Validation
📁 Separate User Database
📚 Book Categories
📅 Different Due Dates for Different Books
🖥️ Improved User Interface
👩‍💻 Author

Poomalar R

🌱 Embedded Systems Enthusiast
💻 C Programmer
🎓 B.E. Electrical and Electronics Engineering
🔧 Embedded C
🐧 Linux
⚡ Embedded Systems

GitHub: https://github.com/poomalar258-code

📄 License

This project is licensed for educational and learning purposes only. You are free to use, modify, and share this project for academic or personal learning with proper credit to the author.

⭐ If you found this project helpful, consider giving it a Star on GitHub!
