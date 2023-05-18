# Trees
Trees are non-linear data structures that represent nodes connected by edges. Each tree consists of a root node as the Parent node, and the left node and right node as Child nodes.

## Why Trees Matter
Trees provide an organized and hierarchical way to store and represent data. They are particularly useful in scenarios where data has a natural hierarchical structure, such as file systems, organization charts, or family trees. By understanding trees, I can gain insights into efficient data organization, searching, and manipulation techniques that can be applied to solve real-world problems.



## Binary tree
A tree whose elements have at most two children is called a binary tree. Each element in a binary tree can have only two children. A node’s left child must have a value less than its parent’s value, and the node’s right child must have a value greater than its parent value.

## Implementation
Here we have created a node class and assigned a value to the node.

```
# node class
class Node:

    def __init__(self, data):
        # left child
        self.left = None
        # right child
        self.right = None
        # node's value
        self.data = data

    # print function
    def PrintTree(self):
        print(self.data)

root = Node(27)

root.PrintTree()
```

## Insertion

The insert method compares the value of the node to the parent node and decides whether to add it as a left node or right node.

Remember: if the node is greater than the parent node, it is inserted as a right node; otherwise,​ it’s inserted left.

Finally, the PrintTree method is used to print the tree.

```
class Node:

    def __init__(self, data):

        self.left = None
        self.right = None
        self.data = data

    def insert(self, data):
# Compare the new value with the parent node
        if self.data:
            if data < self.data:
                if self.left is None:
                    self.left = Node(data)
                else:
                    self.left.insert(data)
            elif data > self.data:
                if self.right is None:
                    self.right = Node(data)
                else:
                    self.right.insert(data)
        else:
            self.data = data

# Print the tree
    def PrintTree(self):
        if self.left:
            self.left.PrintTree()
        print( self.data),
        if self.right:
            self.right.PrintTree()

# Use the insert method to add nodes
root = Node(27)
root.insert(14)
root.insert(35)
root.insert(31)
root.insert(10)
root.insert(19)


root.PrintTree()
```

## Things I want to know more about
How are trees used in database systems?
Can trees be used to represent hierarchical data in graphical user interfaces (GUIs)?
Are there any advanced tree structures or algorithms that are commonly used in real-world applications?
What are the trade-offs between different types of trees, such as binary search trees versus balanced trees?
Are there any practical examples or case studies where tree structures have significantly improved performance or efficiency in solving complex problems?
