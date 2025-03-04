# Technical Writing Assignment

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/fullstack-curriculum/how-tos/working-with-assignments#how-to-work-on-assignments).

## Prompt 1

Arrays, Linked Lists and Doubly Linked Lists all allow programmers to organize data in a sequence. So, how would you choose to use one over the other?

In your response, make sure to compare the time complexities for insertion, removal, and random access (grabbing a particular known element by index/position) for each data structure as well as memory usage and ease of traversal.

### Response 1

## Prompt 2

Imagine you are developing a web browser's "back" button functionality. When a user clicks "back," the browser should navigate to the previously visited webpage.

Would you use a stack or a queue to implement this functionality?

In your response, explain what a Stack/Queue is and why it would be best for this use case. Make sure that your response includes the terms LIFO or FIFO.

### Response 2

```
If I were creating a website and was tasked to create a back button, I would thought of this 'back' button functionality as like a stack. The reason that I say it more of a stack it because of the nature of a stack. Stack follow a rule of FIFO which means that the first element that gets passed into the stack is also the first element that gets removed from the stack. Applying that logic to a website and its 'back' button, you would want to return to the most recent page you visited when you press the back button.
```

## Prompt 3

What is an Abstract Data Type and why are they worth learning about?

### Response 3

## Prompt 4

A few classic problems involving a stack are the `isBalanced` and `isPalindrome` functions. Choose one of these functions and provide a solution to it along with a brief lesson explaining how it works.

### Response 4

For the function 'isPalindrome', essentially what you need to do is see if the given string is the same string if it were backwards. The first step is to make sure that all of the characters in the string are lowercase. This allows for there to be a consistency amongst the elements in the string.

It'll look like this

```js
function isPalindrome(str) {
  // can't forget to create the stack
  const stack = [];

  //turn all the elements into lowercase
  const newString = str.toLowercase();
}
```

Next you want to iterate through the new string and store every value inside the stack using .push

```js
function isPalindrome(str) {
  const stack = [];

  const newString = str.toLowercase();

  //the iteration and placement of characters and placing them inside the stack

  for (let char in newString) {
    stack.push(char);
  }
}
```

after the iteration and insertion, We are now going to **_pop_** out of the stack and check to **newsString.pop()** is equal to char.

```js
function isPalindrome(str) {
  const stack = [];

  const newString = str.toLowercase();

  for (let char of newString) {
    stack.push(char);
  }

  //if statements that check to see if the chars match from inside the stack and the original string

  for (let char of newString) {
    // if the the stacks char is not equal to the original strings char, return false

    if (char !== newString.pop()) {
      return false;
    }
  }
  // returns true only if the stacks  elements match the strings element

  return true;
}
```

That about it folks. I hope you found this useful. good night America
