# Library-Management-System
## Overview
The Library Management System is a console-based application developed as a term project for the Programming Fundamentals course. This system is designed to manage the various functions of a library, including book storage, retrieval, lending, and return. It ensures efficient management of library resources and user interactions.

## Features
1. **User Authentication**:
   - Login and Sign-Up functionality.
   - Registered users can access the system's features.
   - Proper messages displayed for unregistered users with prompts to sign up.

2. **Main Menu**:
   - Provides access to various system features.
   - System remains active until explicitly terminated by the user.
   - Option to return to the menu or re-execute functions after each operation.

3. **Book Storage**:
   - Books have attributes: title, ISBN number, author, date of publishing, quantity available, and total quantity.
   - Stored in text files on local storage.

4. **Book Retrieval**:
   - Search for books by title or ISBN number.

5. **Book Management**:
   - Add new books to the library database.
   - Delete books from the database.

6. **Book Lending and Returning**:
   - Lend books to users.
   - Return issued books.
   - Track late returns and calculate fines.

## Requirements
- **Data Structures**:
  - Use structs for Book and Lending.
  - Book struct: title, ISBN number, author, date of publishing, quantity available, and total quantity.
  - Lending struct: issued Book, issuing date, date of return, borrower's name, and applicable fine.

- **File Storage**:
  - Store lending and book structs in respective directories (Lending and Books).
  - Use `readdir()` function for file access.

- **Capacity Management**:
  - Library capacity: 10,000 books.
  - Maintain arrays of structs for Books and Lendings in memory.
  - Data should be synchronized with text files upon program start, book addition, and deletion.

- **Data Integrity**:
  - Ensure changes in memory are reflected in files.
  - Maintain data integrity between memory and disk storage.

- **Quantity Management**:
  - Decrease available quantity when a book is issued.
  - Prevent issuing if book quantity is zero.
  - Decrease total quantity when a book is deleted.

- **Fine Collection**:
  - Track fines for late returns.
  - Add fines to library's treasury upon late return.

- **Persistent Storage**:
  - Ensure data is not lost upon system closure.
  - Load/reload data automatically on system start or database changes.

- **Efficient Searching**:
  - Implement efficient book search (sorting & binary search).

## Bonus Marks
- Implement a Graphical User Interface (GUI) for additional credit.

## Development Environment
- **IDE**: Visual Studio Community Edition.
- **Language**: C++ (without using STL libraries, OOP concepts, or dynamic memory allocation).

## Installation
1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-repo/library-management-system.git
   ```
2. **Open in Visual Studio**
   - Open Visual Studio Community Edition.
   - Select `Open a project or solution`.
   - Navigate to the cloned repository and open the project file.

3. **Build and Run**
   - Build the project.
   - Run the application.

## Usage
1. **Authentication**
   - Login or sign up to access the system.
   - Follow prompts for new user registration.

2. **Main Menu**
   - Navigate through the main menu to access different features.
   - Follow on-screen instructions for each operation.

3. **Book Management**
   - Add or delete books through the menu options.
   - Ensure to provide all required book details.

4. **Book Retrieval**
   - Search for books by title or ISBN number.

5. **Lending and Returning Books**
   - Issue books to users and return them as per the system prompts.
   - Record late returns and apply fines if applicable.
