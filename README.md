# Local Library: Qualified Assessment

## 1. Project Plan
This project requires the implementation of functionality that will allow users to interact with data of a local library website. The structure of the project has already been provided. The scope of my work is to write javascript that will complete the functionality per the project's requirements. 

### Functions & Features
*   **`findAccountById()`:** Use `find()` to search for accounts using the account id number.
*   **`sortAccountsByLastName()`:** Use `sort()` to sort a collection of accounts by the account holders last name.
*   **`getAccountFullNames()`:** Use `map()` to pull the full name associated with a given account.
*   **`findAuthorById()`:** Use `find()` to search for Author using the author id number. 
*   **`findBookById()`:** Use `find()` to search for books using the book id number
*   **`getTotalBooksCount()`:** Use `books.length` to return the total number of objects that represent the collection of books
*   **`getTotalBooksCount()`:** Use `books.length` to return the total number of objects that represent the collection of books
*   **`getTotalAccountsCount()`:** Use `accounts.length` to return the total number of objects that represent the active accounts 
*   **`getBooksBorrowedCount()`:** Use `filter` to reveal the number of books that are currently being borrowed

---

## 2. Implementation Plan

*   **Step 1: Setup & Initialization** - Download and intialize the code base to local repo using VS Code. 
*   **Phase 2: Core Development** - Read through project requirements, identify javascript functions that need to be written, write functions according for home, books, and accounts sections of the site.
*   **Phase 3: Test & Debug** - Test code via test scripts and npm.

---

## 3. Navigation Structure

This is a very simple site where each page is accessible from a global sticky top navigation bar. 

*   **Entry Point/Overall Stats:** The home page holds general stats concerning details about the inventory and borrowing history.
*   **Stats by Book:** This page contains information on borrow status and details of each book.
*   **Stats by Account:** This page contains account holder information and any books that they are current borrowing.
---

## 4. Justifications & Trade-offs

**Trade-off 1: Longer code for better functionality** 
*   For the `sortAccountsByLastName(accounts)` function, I decided to include `lowercase()` to ensure that the names would be sorted properly regardless of the case it they use when input.
**Trade-off 2: Longer code for better readbility**
*   For the `getBooksBorrowedCount(books)` function, I decided to add one extra line of code to destructure and expose the `{borrows}` array to make the function beneath it more readable.

---

## 5. Challenges & Troubleshooting

The biggest challenge I faced was figuring out how to get the `getBooksBorrowedCount(books)` function to work. The function requires accessing data nested within two objects and two arrays. I first approached this function with a combination of a `map()` and `filter()` function. However, this would always return total number of items in the array rather than a filtered number. This is because the `map()` function would return every array regardless of whether the information had been filtered out of it. Once I discovered this, I resorted to using two levels of the `filter()` function; one to filter through the objects in the array that I needed to access, and the other to make sure that they displayed only the top level objects that contained filtered content.


---

## 6. AI Tools Documentation

| AI Tool | Purpose / How it was Used | Justification for Use |
| :--- | :--- | :--- |
| Google Gemini | Debugging errors | Accelerated troubleshooting |
| CodeGPT | Autocomplete code suggestions | Enhanced development speed |

---

## 7. Project Process Summary

*   **Project Structure:** A sound structure of the project was already established with the completed HTML code provided. I only needed to write the approriate Javascript functionality.
*   **Writing Functions:** I began by identifying the simplest functions and completing those first. Then moving on to write the more complex functions. I leaned on CodeGPT for code suggestions, making sure to review the logic before accepting and implementing each code snippet.
*   **Troubleshooting/Debugging:** Most of the requirements were simple enough to execute upon without issue. However, most of the dev effort was put towards debugging the `getBooksBorrowedCount(books)` function. This function required accessing data that was nested deeply within multiple arrays and objects.

---

## 8. GitHub Commit History

https://github.com/marcusdavisjr/local-library-assessment/commits/main/