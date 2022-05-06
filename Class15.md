# Class15 Reading Notes

Some ideas for how you might want to teach:

Use an analogy
Explain a detail in depth
Use WHY, WHAT, HOW structure
Tutorial / walk through an example
Write a quiz
Create a vocabulary/definition list
Write a cheat sheet
Create a diagram / visualization / cartoon of a topic
Anthropomorphize the concepts, and write a conversation between them
Build a map of the information
Construct a fill-in-the-blank worksheet for the topic

###  Resources
Read: [Trees](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)

**Node** - A Tree node is a component which may contain its own values, and references to other nodes<br>
**Root** - The root is the node at the beginning of the tree<br>
**K** - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.<br>
**Left** - A reference to one child node, in a binary tree<br>
**Right** - A reference to the other child node, in a binary treev
**Edge** - The edge in a tree is the link between a parent and child node<br>
**Leaf** - A leaf is a node that does not have any children<br>
**Height** - The height of a tree is the number of edges from the root to the furthest leaf<br>

Traversing a tree allows us to search for a node, print out the contents of a tree, and much more! There are two categories of traversals when it comes to trees:

**Depth First**

Depth first traversal is where we prioritize going through the depth (height) of the tree first. There are multiple ways to carry out depth first traversal, and each method changes the order in which we search/print the root

**Breadth First**

Breadth first traversal iterates through the tree by going through each level of the tree node-by-node. 

**Binary Trees** restrict the number of children to two (hence our left and right children).

**K-ary Trees**
If Nodes are able have more than 2 child nodes, we call the tree that contains them a K-ary Tree. In this type of tree we use K to refer to the maximum number of children that each Node is able to have.

**Big O**

The Big O time complexity for inserting a new node is O(n). Searching for a specific node will also be O(n). Because of the lack of organizational structure in a Binary Tree.

The Big O space complexity for a node insertion using breadth first insertion will be O(w), where w is the largest width of the tree. 

The Big O time complexity of a Binary Search Tree’s insertion and search operations is O(h)

The Big O space complexity of a BST search would be O(1). During a search, we are not allocating any additional space.

**Binary Search Trees**

A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.

----

## Things I want to know more about

----
[Home](https://github.com/MISalz/401_Reading_Notes/blob/main/README.md)