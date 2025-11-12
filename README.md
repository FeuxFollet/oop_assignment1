# Library Management System

## Project Overview

This project involves a Python program that manages a library system, which is available in both a prodecural version (`library_procedural.py`) and an OOP version (`library_oop.py`)

## Project Structure

- `library_oop.py` : Contains the OOP version of the Library Management System
- `library_procedural.py` : Contains the procedural version of the Library Management System
- `test_oop.py` : Currently an empty file since all the testing are done on the main file (`library_oop.py`)
- `test_procedural.py` : Currently an empty file since all the testing are done on the main file (`test_procedural.py`)

## Book Class

Represent a book.

### Attributes

- `id` (int): Unique ID to identify the book.
- `title` (str): Title of the book.
- `author` (str): Author of the book.
- `total_copies` (int): Total number copies in the library.
- `available_copies` (int): Total number of copies available to borrow.

## Member Class

Represent a library member.

### Attributes

- `id` (int): Unique ID to identify the member.
- `name` (str): Name of the member.
- `email` (str): E-mail address of the member.
- `borrowed_books_list` (list): List of book borrowed by the member.

## Library CLass

Collection of all boks and members, also manages all library operations.

### Attributes

- `books` (list): List of all books in the library.
- `members` (list): List of all library members.

### Methods

- `add_book(book_id, title, author, available_copies)`: Add a new book to the library.
- `add_member(member_id, name, email)`: Add a new member into the library.
- `find_book(book_id)`: Searches for a book by it's ID (`book_id`).
- `find_member(member_id)`: Searches for a member by the ID (`member_id`).
- `borrow_book(member_id, book_id)`: Allows a member to borrow a book (if available).
- `return_book(member_id, book_id)`: Allows a member to return a borrowed book.
- `display_available_books()`: Display all the books in the library.
- `display_member_books(member_id)`: Display all the books currently borrowed by that member ID (`member_id`)

## Running the program

To run the OOP version of the program, execute `library_oop.py`:

```bash
python library_oop.py
```

To run the prodecural version of the program, execute `library_procedural.py`:

```bash
python library_procedural.py
```