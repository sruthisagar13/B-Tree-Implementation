# B-Tree-Implementation
Implementation of B+ Tree in RDBMS 

Implementing B+ tree using C++

 Search
 Insert
 Structuring the main Function
 Delete
 
 **Usage :**
Clone it to some place in your PC.
Install Visual Studios Community Edition -2019.
File->create new project with existing code.

**Summary- What is the project all about?**

This project is small version of database system. Where we efficiently implement the B+ Tree for fast and efficient access of files in the disc. Your database tuples will be stores as a .txt file in DBFiles folder corresponding FILE* will be saved in the leaf node. Above step is done to mimic the disc-block access. (TO-DO Delete the files in DBFiles folder after each run). If we want to make more tables then we can make that many BPTree objects !!

**Assumptions in our Tree :**

We are making a right biased tree. By this we mean if maxLimits are even we will split them in such a way that right sibling has one element greater.

Insertion is based on the primary key. Hence all the properties of the primary key has to be followed. No dublicate insertion has to be done with same primary key!

In the code we have used a ptr2parent which directly give access to the parent of the node with ease, which is little bit deviated from B+ Tree defination where we don't use it. Consequences of this are yet to be unfold. Meanwhile, I have added it as a question in stackoverflow (NOW IT HAS BEEN REMOVED AS IT WILL CREATE A MESS WHILE DELETION).

We are saving the *ptr2next explicitly while ideally it is saved as the last pointer in the pointerset. But here as we are using union to save the memory and seperate the leaf and non-leaf nodes, because of this *ptr2next is explicitly saved !!



