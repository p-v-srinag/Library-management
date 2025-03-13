Key Structures:
Book structure (struct book):

name: Name of the book.
author: Author of the book.
id: Unique identifier for each book.
next: Pointer to the next book in the list (linked list structure).
Student structure (struct student):

name: Name of the student.
email: Email of the student.
book: Name of the book issued to the student.
a: Author of the book issued.
id: Book ID issued to the student.
next: Pointer to the next student in the list (linked list structure).
Core Functions:
Library Initialization (initialize_lib):

Initializes the library with a set of books (predefined), each with a unique ID, name, and author.
Books are linked in a list.
Book Issue (book_issue):

Displays available books in the library.
Allows the user to enter the Book ID to issue it.
Collects student details (name, email) and issues the book.
The issued book is removed from the library list and added to the student’s record.
Book Return (book_return):

Allows a student to return a book by providing the Book ID.
Searches the student records for the book and removes it from the student’s list.
Adds the returned book back into the library collection.
Display Student Details (display):

Shows the list of students who have issued books, along with the details like the student’s name, email, and the book issued.
Book Deletion (delete_book):

Deletes a book from the library collection, either by removing it entirely or adjusting the list to remove a specific book by ID.
Add New Book (add_book):

Adds a new book to the library collection after a book is returned by a student.
Menu and Greetings:

Main Menu (main_menu): Displays a menu with options to issue books, return books, display student details, or exit the program.
Greetings (greetings): Displays a welcome message when the program starts.
Features:
Linked List Usage:

Both books and students are stored as linked lists (start_lib for books and start for students).
This allows easy traversal and dynamic modification (e.g., adding/removing books or student records).
Book Issue and Return:

Books are dynamically added or removed from the library when issued or returned, keeping the library’s inventory up-to-date.
Student Records:

Each time a student issues or returns a book, a record of the transaction is maintained in the student’s linked list.
