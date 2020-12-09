# Stacks and Queues

What is a Stack
A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

![img](https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2013/03/stack.png)

## The functions associated with stack are:

* empty() – Returns whether the stack is empty – Time Complexity : O(1)
* size() – Returns the size of the stack – Time Complexity : O(1)
* top() – Returns a reference to the top most element of the stack – Time * Complexity : O(1)
* push(g) – Adds the element ‘g’ at the top of the stack – Time Complexity : O(1)
* pop() – Deletes the top most element of the stack – Time Complexity : O(1)

## Stacks follow these concepts:

**FILO**
First In Last Out
This means that the first item added in the stack will be the last item popped out of the stack.

**LIFO**
Last In First Out
This means that the last item added to the stack will be the first item popped out of the stack.

## Implementation

There are various ways from which a stack can be implemented in Python. This article covers the implementation of stack using data structures and modules from Python library. 
Stack in Python can be implemented using following ways: 

* list
* collections.deque
* queue.LifoQueue

### Implementation using list:

Python’s buil-in data structure list can be used as a stack. Instead of push(), append() is used to add elements to the top of stack while pop() removes the element in LIFO order. 
Unfortunately, list has a few shortcomings. The biggest issue is that it can run into speed issue as it grows. The items in list are stored next to each other in memory, if the stack grows bigger than the block of memory that currently hold it, then Python needs to do some memory allocations. This can lead to some append() calls taking much longer than other ones.

### Implementation using queue module

Queue module also has a LIFO Queue, which is basically a Stack. Data is inserted into Queue using put() function and get() takes data out from the Queue.
There are various functions available in this module:

* maxsize – Number of items allowed in the queue.
* empty() – Return True if the queue is empty, False otherwise.
* full() – Return True if there are maxsize items in the queue. If the queue was initialized with maxsize=0 (the default), then full() never returns True.
* get() – Remove and return an item from the queue. If queue is empty, wait until an item is available.
* get_nowait() – Return an item if one is immediately available, else raise QueueEmpty.
* put(item) – Put an item into the queue. If the queue is full, wait until a free slot is available before adding the item.
* put_nowait(item) – Put an item into the queue without blocking.
* qsize() – Return the number of items in the queue. If no free slot is immediately available, raise QueueFull.

### Implementation using singly linked list

The linked list has two methods addHead(item) and removeHead() that run in constant time. These two methods are suitable to implement a stack. 

getSize()– Get the number of items in the stack.
isEmpty() – Return True if the stack is empty, False otherwise.
peek() – Return the top item in the stack. If the stack is empty, raise an exception.
push(value) – Push a value into the head of the stack.
pop() – Remove and return a value in the head of the stack. If the stack is empty, raise an exception.
