# Threaded Binary Search Tree - File Management System

A console-based File Management System implemented in C++ using a **Threaded Binary Search Tree (TBST)**. This project demonstrates advanced pointer manipulation and data structures by optimizing tree traversals without using recursion or an explicit stack.

## Features
* **Add File:** Insert file records (Name, Size, Type) into the BST.
* **Delete File:** Safely remove files handling all three BST deletion cases (leaf nodes, single-child nodes, and two-child nodes).
* **Inorder Traversal:** List all files alphabetically in $O(1)$ extra space using thread pointers.

## Core Data Structure
Standard Binary Search Trees waste half of their pointer fields on `nullptr`. This project utilizes a **Threaded BST**, where:
* `lthread` and `rthread` boolean flags indicate whether a pointer leads to a child or an in-order predecessor/successor.
* Traversals run without a call stack or auxiliary stack memory.

## How to Compile and Run

Make sure you have a C++ compiler installed (like `g++`).

```bash
# Compile the code
g++ -o file_manager main.cpp

# Run the program
./file_manager
