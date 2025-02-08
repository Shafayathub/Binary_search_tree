# Binary Search Tree (BST) Rules

A **Binary Search Tree (BST)** is a type of binary tree that follows a specific ordering property.

###all values of the left sub-tree < node->val.
###all values of right sub-tree > node->val.
###BST duplicate can't be inserted rather we keep a count of the element.

## Rules of a Binary Search Tree

1. **Node Structure**
   - Each node has at most two children: a **left child** and a **right child**.

2. **Ordering Property**
   - The **left subtree** of a node contains only nodes with values **less than** the node’s value.
   - The **right subtree** of a node contains only nodes with values **greater than** the node’s value.
   - No duplicate values are allowed in a strict BST.

3. **Recursive Property**
   - The left and right subtrees must also be **binary search trees**.

4. **Traversal Invariant**
   - An **in-order traversal** (Left, Root, Right) of a BST results in a **sorted sequence** of values.

5. **Performance (Time Complexity)**
   - **Search**: \( O(\log n) \) in a balanced BST, \( O(n) \) in an unbalanced BST.
   - **Insertion**: \( O(\log n) \) in a balanced BST, \( O(n) \) in an unbalanced BST.
   - **Deletion**: \( O(\log n) \) in a balanced BST, \( O(n) \) in an unbalanced BST.

## Example BST

```
        50
       /  \
     30    70
    /  \   /  \
   20  40 60  80
```

## Edge Cases
- **Skewed Tree**: If elements are inserted in increasing or decreasing order, the tree becomes skewed (like a linked list), resulting in \( O(n) \) time complexity.
- **Balanced Tree**: A self-balancing BST (e.g., AVL Tree, Red-Black Tree) ensures \( O(\log n) \) operations.

## Applications of BST
- Searching and sorting
- Implementing associative arrays (e.g., map, set)
- Database indexing
- Network routing algorithms

## Conclusion
A Binary Search Tree is an efficient data structure for searching, inserting, and deleting elements while maintaining a sorted structure. However, maintaining balance is crucial for optimal performance.
