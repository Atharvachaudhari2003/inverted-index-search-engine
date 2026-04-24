# Inverted Index Search Engine

## Description

This project implements an efficient text search system using the concept of an inverted index, a fundamental technique used in modern search engines. Instead of scanning entire documents sequentially for every query, the system builds a structured mapping of words to the documents in which they appear. This approach significantly improves search speed and efficiency, especially when handling large datasets.

The system processes multiple text files as input, reads their content using file handling techniques in C, and performs tokenization to extract meaningful words. These words are then stored in a data structure such as a linked list or hash table, where each word is associated with a list of documents and its frequency of occurrence. This mapping forms the inverted index, which allows quick lookup during search operations.

When a user enters a query, the system directly accesses the indexed data instead of scanning all files, thereby reducing the overall search time complexity. Compared to traditional linear search methods with O(n) complexity, this system achieves near O(1) lookup time when hashing is used. The search is also case-insensitive, making it more user-friendly and practical.

---

## Features

* Fast keyword-based document search
* Efficient inverted index creation
* Supports multiple input files
* Case-insensitive searching
* Displays word frequency and document occurrence

---

##  Technologies Used

* C Programming Language
* File Handling
* Data Structures (Linked List / Hashing)

---

## Project Structure

```
inverted-search/
│── src/
│   ├── main.c
│── include/
│── data/
│   ├── file1.txt
│   ├── file2.txt
│── README.md
```

---

## How to Run

1. Compile the program:

```
gcc main.c -o search
```

2. Run the executable:

```
./search file1.txt file2.txt
```

3. Enter search query when prompted.

---

## How It Works

1. Reads multiple text files
2. Tokenizes words from each file
3. Builds inverted index (word → file list)
4. Stores frequency of each word
5. On query, retrieves results instantly

---

## Applications

* Search engines
* Document retrieval systems
* Text analysis tools

---

##  Outcome

This project demonstrates how proper use of data structures can drastically improve system performance. It provides a strong foundation in file processing, memory management, and algorithm optimization, making it highly relevant for real-world applications involving large-scale text data.

---

## Future Enhancements

* GUI-based search interface
* Support for large datasets using files/databases
* Ranking of search results
* Phrase search support

---

##  Author

Atharva Chaudhari
