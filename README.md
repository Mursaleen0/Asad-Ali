# AVL Tree Implementation in C++

This project implements an AVL Tree in C++, a self-balancing binary search tree where the difference between the heights of left and right subtrees cannot be more than one for all nodes.

## Features
- **Self-balancing:** Automatically balances itself during insertions to ensure O(log n) time complexity for search, insert, and delete operations.
- **Rotations:** Implements left and right rotations to maintain balance.
- **Traversal:** Supports inorder traversal to print the elements in sorted order.

## Code Structure

### Class `AVLTree`
The main class encapsulating the AVL Tree logic.

#### Private Members
- **Struct `Node`:** Represents a node in the AVL tree.
  - `int key`: The key value of the node.
  - `Node* left`: Pointer to the left child.
  - `Node* right`: Pointer to the right child.
  - `int height`: Height of the node.
  
- **Node* root:** Pointer to the root node of the AVL tree.

- **Helper Functions:**
  - `int getHeight(Node* node)`: Returns the height of a given node.
  - `int getBalanceFactor(Node* node)`: Computes the balance factor of a node.
  - `Node* rotateRight(Node* y)`: Performs right rotation on a given node.
  - `Node* rotateLeft(Node* x)`: Performs left rotation on a given node.
  - `Node* insert(Node* node, int key)`: Recursively inserts a key into the subtree rooted with a given node.
  - `void inorderTraversal(Node* node)`: Recursively performs inorder traversal of the subtree rooted with a given node.

#### Public Members
- **Constructor:**
  - `AVLTree()`: Initializes an empty AVL tree.
  
- **Public Methods:**
  - `void insert(int key)`: Inserts a key into the AVL tree.
  - `void printInorder()`: Prints the keys of the AVL tree in inorder traversal.

### Main Function
- **main()**: Demonstrates the usage of the AVL tree by inserting some keys and printing the inorder traversal.

## Usage

1. **Compilation:**
   ```sh
   g++ -o avltree avltree.cpp
This is a change in the forked repo.
