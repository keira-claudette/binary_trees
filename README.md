# Data Structures Binary trees
The following data structures are used for binary trees in this repository.
### Basic Binary Tree
```
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
```

### Binary Search Tree
``` typedef struct binary_tree_s bst_t; ```

### AVL Tree
``` typedef struct binary_tree_s avl_t; ```

### Max Binary Heap
``` typedef struct binary_tree_s heap_t; ```

###### Note: All files dealwith simple binary trees, they are not BSTs thus they don't follow any kind of rule.


# Files

- ##### 0-binary_tree_node.c
creates a binary tree node. <br>
prototype: `binary_tree_t *binary_tree_node(binary_tree_t *parent, int value);`

- ##### 1-binary_tree_insert_left.c
Inserts a node as the left-child of another node.<br>
Prototype: `binary_tree_t *binary_tree_insert_left(binary_tree_t *parent, int value);`

- ##### 2-binary_tree_insert_right.c
Inserts a node as the right-child of another node. <br>
Prototype: `binary_tree_t *binary_tree_insert_right(binary_tree_t *parent, int value);`

- ##### 3-binary_tree_delete.c
Deletes an entire binary tree. <br>
Prototype: `void binary_tree_delete(binary_tree_t *tree);`

- ##### 4-binary_tree_is_leaf.c
Checks if a node is a leaf. <br>
Prototype: `int binary_tree_is_leaf(const binary_tree_t *node);`

- ##### 5-binary_tree_is_root.c
Checks if a given node is a root.<br>
Prototype: `int binary_tree_is_root(const binary_tree_t *node);`

-  ##### 6-binary_tree_preorder.c
Describes a function that goes through a binary tree using pre-order traversal <br>
Prototype: `void binary_tree_preorder(const binary_tree_t *tree, void (*func)(int));`

- ##### 7-binary_tree_inorder.c
Describes a function that goes through a binary tree using in-order traversal. <br>
Prototype: `void binary_tree_inorder(const binary_tree_t *tree, void (*func)(int));`

- ##### 8-binary_tree_postorder.c
Describes a function that goes through a binary tree using post-order traversal. <br>
Prototype: `void binary_tree_postorder(const binary_tree_t *tree, void (*func)(int));`

- ##### 9-binary_tree_height.c
Describes a function that measures the height of a binary tree. <br>
Prototype: `size_t binary_tree_height(const binary_tree_t *tree);`

- ##### 10-binary_tree_depth.c
Describes a function that measures the depth of a node in a binary tree <br>
Prototype: `size_t binary_tree_depth(const binary_tree_t *tree);`

- ##### 11-binary_tree_size.c
Describes a function that measures the size of a binary tree<br>
Prototype: `size_t binary_tree_size(const binary_tree_t *tree);`

- ##### 12-binary_tree_leaves.c
Describes a function that counts the leaves in a binary tree. <br>
Prototype: `size_t binary_tree_leaves(const binary_tree_t *tree);`

- ##### 13-binary_tree_nodes.c
Describes: a function that counts the nodes with at least 1 child in a binary tree<br>
Prototype: `size_t binary_tree_nodes(const binary_tree_t *tree);`

- ##### 14-binary_tree_balance.c
Describes a function that measures the balance factor of a binary tree. <br>
Prototype: `int binary_tree_balance(const binary_tree_t *tree);`

- ##### 15-binary_tree_is_full.c
Describes a function that checks if a binary tree is full.<br>
Prototype: `int binary_tree_is_full(const binary_tree_t *tree);`

- ##### 16-binary_tree_is_perfect.c
Describes a function that checks if a binary tree is perfect. <br>
Prototype: `int binary_tree_is_perfect(const binary_tree_t *tree);`

- ##### 17-binary_tree_sibling.c
Describes a function that finds the sibling of a node. <br>
Prototype: `binary_tree_t *binary_tree_sibling(binary_tree_t *node);`

- ##### 18-binary_tree_uncle.c
Describes a function that finds the uncle of a node. <br>
Prototype: `binary_tree_t *binary_tree_uncle(binary_tree_t *node);`