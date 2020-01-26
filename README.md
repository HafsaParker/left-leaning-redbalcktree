# left-leaning-leftbalcktree
A left leaning Red Black Tree or (LLRB), is a variant of red black tree, which is a lot easier to implement than Red black tree itself and guarantees all the search, delete and insert operations in O(logn) time.

# INSERTION:

While inserting a new node, the new node is always inserted as a RED node. After insertion of a new node, if the tree is violating the properties of the red-black tree then, we do the following operations.
      1.Recolor
      2.Rotation
   # CHARACTERSTICS OF LEFT LEANING RED BLACK TREE:
       1. Root node is Always BLACK in color.

       2. Every new Node inserted is always RED in color.

       3. Every NULL child of a node is considered as BLACK in color.

       4. There should not be a node which has RIGHT RED child and LEFT BLACK child(or NULL child as all NULLS are BLACK), if present Left         rotate the node, and swap the colors of current node and its LEFT child so as to maintain consistency for rule 2 i.e., new node             must be RED in color.

       5. There should not be a node which has LEFT RED child and LEFT RED grandchild, if present Right Rotate the node and swap the colors         between node and it’s RIGHT child to follow rule 2.

       6. There should not be a node which has LEFT RED child and RIGHT RED child, if present Invert the colors of all nodes i. e.,                  current_node, LEFT child, and RIGHT child.

 # DELETION:

 Deleting a node may or may not disrupt the red-black properties of a red-black tree. If this action violates the red-black properties,     then a fixing algorithm is used to regain the red-black properties.
This algorithm is implemented when a black node is deleted because it violates the black depth property of the red-black tree.
This violation is corrected by assuming that node x (which is occupying y's original position) has an extra black. This makes node x   neither red nor black. It is either doubly black or black-and-red. This violates the red-black properties.
However, the color attribute of x is not changed rather the extra black is represented in x's pointing to the node.

The extra black can be removed if:

    1.It reaches the root node.

    2.If x points to a red-black node. In this case, x is colored black.

    3.Suitable rotations and recolorings are performed
  # collaborated by 
  @HibabKhan and @HafsaParker

