# Student Library Management System

A simple C-based program that simulates a library management system for students. The system allows students to issue and return books, and it keeps track of student and book details using linked lists.

## Features

- **Book Issue**: Students can issue books by providing their details and selecting a book from the library.
- **Book Return**: Students can return books, and the system updates the book inventory.
- **Student Record**: The program maintains a record of students who have issued books, including their name, email, and book details.
- **Dynamic Book Management**: Books are dynamically added or removed from the library collection based on issue and return actions.
- **Simple Text-based Interface**: The program uses a menu-driven interface for user interaction.

## Installation

To use this program, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Library-Management-System.git
Navigate to the project directory:

         cd Library-Management-System
   
Compile the C program:

         gcc -o library_system main.c
   
Run the program:

         ./library_system
   
How It Works:

Book Initialization
The program initializes a set of books at the start, each with the following details:

Book Name
Author
Book ID
Main Menu
Once the program starts, a greeting message is displayed, and the main menu is shown with the following options:

Issue Book: Allows a student to issue a book by providing their name, email, and selecting a book ID.
Return Book: Allows a student to return a book by providing the Book ID.
Display Student Details: Displays details of all students who have issued books.
Exit: Exits the program.

Book Issue
The student selects a book by its Book ID.
The system prompts for the student's name and email.
The selected book is issued to the student, and it is removed from the library's available books.

Book Return
The student enters their Book ID to return the book.
The system updates the student's record and adds the returned book back to the library.
Display Student Details
Displays a list of all students who have issued books, along with their personal details and the books they have borrowed.


Example Output

         Main Menu:
         
         *************************************************
               MAIN MENU:
              1. ISSUE OF BOOKS
              2. RETURN OF BOOKS
              3. DISPLAY STUDENT DETAILS
              4. EXIT
         *************************************************
               Enter your choice: 
         
         Book Issue:
         
         *************** Books Available: ****************
         
         _________________________________________________
          Book 1
          Book Title: The Kite Runner
          Name of Author: Khaled Hosseini
          Book ID: 101
         _________________________________________________
         Enter the Book ID: 101
         Enter Student Details:
          Enter your Name: John Doe
          Enter your Email: john.doe@example.com
         Issue of Book ID 101 done successfully!
         
         Book Return:
         
         
         *************** Books Submission: ****************
         
         Enter your Book ID: 101
         Student Name: John Doe
         Student Email: john.doe@example.com
         Name of Book Issued: The Kite Runner
         Book ID: 101
         Return of Book ID 101 done successfully!

Code Structure

main.c: Contains the main logic of the program, including the initialization, book issue, book return, and student record management.
struct book: Defines the book structure with fields for name, author, ID, and a pointer to the next book.
struct student: Defines the student structure with fields for name, email, book details, and a pointer to the next student.

Acknowledgements

This project was created to demonstrate basic data structures (linked lists) in C programming.
Special thanks to all the open-source contributors who have inspired this project.
