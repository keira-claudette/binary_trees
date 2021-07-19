# Data Structures Binary trees
The following data structures are used for binary trees in this repository.
### Basic Binary Tree
'''
/**
 * struct binary_tree_s - Binary tree node
 *
 * @n: Integer stored in the node
 * @parent: Pointer to the parent node
 * @left: Pointer to the left child node
 * @right: Pointer to the right child node
 */
struct binary_tree_s
{
    int n;
    struct binary_tree_s *parent;
    struct binary_tree_s *left;
    struct binary_tree_s *right;
};

typedef struct binary_tree_s binary_tree_t;
'''

### Binary Search Tree
''' typedef struct binary_tree_s bst_t; '''

### AVL Tree
''' typedef struct binary_tree_s avl_t; '''

### Max Binary Heap
''' typedef struct binary_tree_s heap_t; '''

###### All files dealwith simple binary trees, they are not BSTs thus they don't follow
 any kind of rule.


# Files

- ##### 0-binary_tree_node.c
creates a binary tree node.
prototype: `binary_tree_t *binary_tree_node(binary_tree_t *parent, int value);`

- ##### 1-binary_tree_insert_left.c
Inserts a node as the left-child of another node.
Prototype: `binary_tree_t *binary_tree_insert_left(binary_tree_t *parent, int value);`

- ##### 2-binary_tree_insert_right.c
Inserts a node as the right-child of another node
Prototype: `binary_tree_t *binary_tree_insert_right(binary_tree_t *parent, int value);`

- ##### 3-binary_tree_delete.c
Deletes an entire binary tree.
Prototype: `void binary_tree_delete(binary_tree_t *tree);`

- ##### 4-binary_tree_is_leaf.c
Checks if a node is a leaf.
Prototype: `int binary_tree_is_leaf(const binary_tree_t *node);`

- ##### 5-binary_tree_is_root.c
Checks if a given node is a root.
Prototype: `int binary_tree_is_root(const binary_tree_t *node);`
