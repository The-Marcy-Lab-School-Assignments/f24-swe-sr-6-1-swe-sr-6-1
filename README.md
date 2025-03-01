# Technical Writing Assignment

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/fullstack-curriculum/how-tos/working-with-assignments#how-to-work-on-assignments).

## Prompt 1

Arrays, Linked Lists and Doubly Linked Lists all allow programmers to organize data in a sequence. So, how would you choose to use one over the other?

In your response, make sure to compare the time complexities for insertion, removal, and random access (grabbing a particular known element by index/position) for each data structure as well as memory usage and ease of traversal.

### Response 1

I would choose an array if I need fast random access, working with contiguous memory, and have mostly static data or frequent access by index.

I would choose a singly linked list if I need frequent insertions/removals at the beginning or end and don't need backward traversal.

And I would choose a doubly linked list when I need to move in both directions and frequently add or remove things in the middle.

## Prompt 2

Imagine you are developing a web browser's "back" button functionality. When a user clicks "back," the browser should navigate to the previously visited webpage. 

Would you use a stack or a queue to implement this functionality? 

In your response, explain what a Stack/Queue is and why it would be best for this use case. Make sure that your response includes the terms LIFO or FIFO.

### Response 2

A stack is a data structure that used the LIFO principle. This means that the last item you add is the first one you remove, just like a stack of toy blocks. So when the user visits a new webpage, it gets pushed onto the stack. In contrast queues follow the FIFO principle, meaning the first item added is the first one removed—like people standing in a line. This wouldn't work well for a "back" button because you'd have to return to the very first page before reaching the recent ones. 

## Prompt 3

What is an Abstract Data Type and why are they worth learning about?

### Response 3

## Prompt 4

A few classic problems involving a stack are the `isBalanced` and `isPalindrome` functions. Choose one of these functions and provide a solution to it along with a brief lesson explaining how it works. 

### Response 4



