Download Link: https://assignmentchef.com/product/solved-solvedcomputer-science-230-assignment-4
<br>
Objectives:

to examine and modify a binary search tree ADT

to implement a simplified version of a structure we have learnedabout

Requirements:

Discussed the B+tree, which has all data in the leaves and only keys in the tree. We willsimulate a simplified version of this combination using an array and a binarysearch tree. We will call our version the BMinusTree.

Specifications:

Use the AutoPart class from the previous assignment.

Write a DataBank class that contains an array ofAutoPart objects. The constructorhas a single parameter that says how many objects the array can hold. Themethod insert() has an AutoPart object as its only parameter. The method inserts the object intothe next available place in the array, and returns an int that says where the object was inserted, or -1 if the insert did not work. The method fetch() has an int parameterand returns the AutoPart objectat the position indicated, or null if thereis a problem. The method update() has anint parameter and accesses the AutoPart object at the position indicated, or null if there is a problem. (For the time being there is no delete() method.) The method printArray() has no parameters and prints the contents of the array in physicalorder. This is to be used for debugging only.

The author’scode BinaryTreeWithLNRTraversal (RENAMED BinarySearchTree) is on WebCT. Modify this code to make a tree that holds (only) a partNumber and an index to the AutoPart object of which that is the ID number.

· When a AutoPart objectis inserted into DataBank, its partNumber is inserted into the tree, along with its index (where the objectis in the array).

· When a AutoPart objectis searched for, it is found by finding its partNumber in the tree and using theindex to find the object in the array. (If you just search down the array youwill be penalized.)

· Retain the author’s method LNRoutputTraversal(), which you may need for debugging.

· Add a method printParts()based on LNRoutputTraversal() that prints allof the parts in ascending partNumberorder.

Modify the classPartsStore from the previousassignment to store AutoPartobjects in a BMinusTree.(Don’t write a separate driver; PartsStore is the driver.) Forsimplicity we will allow updates to the price and numberInStockfields only. Be sure that PartsStoreexercises the BMinusTreethoroughly. I reserve the right to replace your PartsStore class with my own test class.

Submission:

Every file thatyou submit must begin with a comment giving the author’s name. If you modifysomeone else’s file, include both the original author’s name and your name.

Submit the files AutoPart, DataBank, BinarySearchTree, and PartsStore onWebCT by the date and time specified above. If you cannot submit on WebCT emailthe files to me. Submit only .java files,not .class files. Do not use a Javapackage. Do not put the files into a folder or, zip the files or use any otherarchive.