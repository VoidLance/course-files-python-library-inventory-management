# Library Inventory Management

A small Python example project for tracking books in a library. It defines `Book` and `Library` classes, with a demonstration of adding books, searching the collection, and changing availability.

## Features

- Add books with a title, author, and availability status.
- Search by exact title or author, ignoring capitalization.
- Update the availability of books by title.
- Print readable book details.

## Getting started

### Requirements

- Python 3.6 or later
- No third-party dependencies

Clone the repository and run the example:

```bash
git clone https://github.com/VoidLance/course-files-python-library-inventory-management.git
cd course-files-python-library-inventory-management
python3 Library_Inventory_Management.py
```

The script creates three sample books, prints the collection, searches for books, and demonstrates changing a book's availability.

### Use the classes

The `Book` constructor adds each new book to the module-level `library` automatically:

```python
from Library_Inventory_Management import Book, library

book = Book("Dune", "Frank Herbert")

matches = library.search_by_title("dune")
print(matches[0])  # Dune by Frank Herbert (available)

library.update_availability("Dune", False)
print(book.available)  # False
```

Importing the module also runs its built-in demonstration and prints its sample output.

## Help

For questions or bug reports, [open an issue](https://github.com/VoidLance/course-files-python-library-inventory-management/issues).

## Maintainers and contributing

This repository is maintained by [@VoidLance](https://github.com/VoidLance). Contributions are welcome: open an issue to discuss a change, or submit a pull request with a focused improvement and a clear description. There is no separate contribution guide or test suite in the repository at this time.
