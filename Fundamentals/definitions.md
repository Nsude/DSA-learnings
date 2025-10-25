## Data Structures
Data structures are ways of organizing and storing data in a computer so it can be used efficiently, depending on the type of data and the operations you need to perform.

## Algorithms
Algorithms are high-level plans and rules that define how the data should be processed or modified, e.g sorting, searching, patching, or deleting.


## Types of Data Structures

<details>
  <summary>🎁 Arrays</summary>

  An array is simply a collection of data stored side-by-side. Like a row of boxes where you can jump from any box to another provided you know the location (index) of the box.

  ````Note:```` At the memory level, arrays have a fixed size. To “grow” an array, a new larger one is created, and the old elements are copied over.
  
  In JavaScript, methods like ```push()``` seem to resize arrays because the JS engine allocates extra space ahead of time and creates a new array only when that space runs out.

</details>

<details>
  <summary>🎁 Queues</summary>

  Queues are just that, queues. They follow a First-In-First-Out principle. This also means that they can only be modified at both ends. Data can only be inserted at the bottom and removed from the top of queues.

</details>

<details>
  <summary>🎁 Stacks</summary>

  Stacks follow a Last-In-First-Out principle. They can only be modified from the top.

  This is how JavaScript's call stack works, the last function that's called is the first one to finish execution.
</details>

<details>
  <summary>🎁 Linked Lists</summary>

  Linked lists are a collection of nodes where each node holds some of data and points to the next node in the collection. 

  There are two kinds of linked lists. ``` singly linked lists: ``` where each node points only to the next node, and ``` doubly linked lists: ``` each node points to the next node and previous node.
</details>

<details>
  <summary>🎁 Hash Tables</summary>

  Hash tables are much like JS objects. they use key: value pairs where the keys serve as references to the data they contain. Hash tables are great for storing data once hashing is good, but they use more memory. 
</details>