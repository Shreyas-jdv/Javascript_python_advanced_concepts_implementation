# Javascript_python_advanced_concepts_implementation
The repository contains solutions to the following problems

1. Implement a deep flatten function which flattens array
or objects and also handles all edge cases of diff data
types.

3. Implement set of functions which can handle 'n async
tasks in series, parallel and race.

5. Implement memoizing or caching identical API request
calls based on route paths.

7. Implement a custom class of Event Emitter model
which can be subscribed to listen and emit events.

9. Implement your custom native javascript promises from
scratch, which emits similar behavior.

11. Implement a currying function accepts 'n number of
arguments which also supports placeholder arguments.

13. Implement the polyfill version of call, apply and bind
functions which handles "this" context.

15. Implement a polyfill of the Object assign method which
copies all enumerable properties from source to target.

============================================================================================

The concepts involved in each problem are defined below

1. Deep Flatten Function
A deep flatten function is a recursive algorithm that takes an input which could be an array (or object) containing nested arrays (or objects) and flattens it into a single, flat array. This process involves traversing all levels of nested structures, extracting all the values, and producing a one-dimensional array.

Key Concepts:
Recursion: The function calls itself on nested elements to flatten them.
Base Case: When the element is neither an array nor an object, it is added to the result directly.
Edge Cases: Handles cases where the input might include other data types like numbers, strings, or even null/undefined values.

2. Handling 'n' Async Tasks in Series, Parallel, and Race
In asynchronous programming, tasks can be executed in various ways to optimize performance and control flow:
Series: Tasks are executed one after another. Each task waits for the previous one to complete before starting.
Parallel: Tasks are executed concurrently without waiting for others to finish. This can lead to significant performance improvements.
Race: The first task to complete (successfully or with an error) will determine the result. This approach is useful when you want the quickest response among several options.
Key Concepts:
Async/Await: Modern asynchronous syntax in languages like Python and JavaScript that makes asynchronous code appear synchronous.
Promises/Futures: Represent a value that may be available now, in the future, or never.
Concurrency vs. Parallelism: Concurrency is about managing multiple tasks at once, while parallelism is about doing multiple tasks simultaneously.

3. Memoizing or Caching Identical API Request Calls
Memoization is an optimization technique where the results of expensive function calls (like API requests) are cached, and subsequent identical calls return the cached result instead of re-executing the function. This technique improves performance, especially in scenarios where the same data is requested frequently.

Key Concepts:
Caching: Temporarily storing data to serve future requests faster.
Key-Value Storage: Cached results are typically stored in a dictionary-like structure, where the API route/path is the key.
Idempotency: An operation where applying it multiple times has the same effect as applying it once. Memoization works well with idempotent operations.

4. Custom Event Emitter Model
An Event Emitter is a pattern used to create and manage events within a system. It allows objects to communicate with each other without being tightly coupled. An event emitter can "emit" or "trigger" events, and other parts of the program can "listen" for these events and respond accordingly.

Key Concepts:
Observer Pattern: The event emitter model is an implementation of the observer pattern, where objects subscribe to events and are notified when they occur.
Event Loop: Especially in environments like JavaScript, event emitters work within the event loop, asynchronously handling events.
Decoupling: It allows different parts of a system to interact with each other without being directly connected, improving modularity and flexibility.

5. Custom Native JavaScript Promises
A Promise in JavaScript is an object representing the eventual completion or failure of an asynchronous operation. Creating a custom promise involves implementing the then, catch, and finally methods that handle the asynchronous logic and state management (pending, fulfilled, rejected).

Key Concepts:
Promise States: A promise can be in one of three states: pending, fulfilled, or rejected.
Chaining: Promises allow chaining, where you can attach multiple handlers to process the results in sequence.
Asynchronous Flow Control: Promises help in managing asynchronous operations more cleanly compared to traditional callback-based approaches.

6. Currying Function with Placeholder Support
Currying is a technique of translating a function that takes multiple arguments into a series of functions that each take a single argument. A curried function allows partial application of arguments, returning a new function that takes the remaining arguments. Placeholder support allows arguments to be skipped and provided later.

Key Concepts:
Partial Application: Allows functions to be invoked with fewer arguments than they expect, returning a new function that takes the remaining arguments.
Higher-Order Functions: Functions that return other functions or take functions as arguments.
Placeholder: A special value that indicates a placeholder for an argument that will be provided later.

7. Polyfill for call, apply, and bind
A Polyfill is code that provides modern functionality on older environments that do not natively support it. The call, apply, and bind methods in JavaScript allow you to explicitly set the this context of a function.
call: Invokes a function with a specified this context and arguments provided individually.
apply: Similar to call, but the arguments are provided as an array.
bind: Returns a new function that, when invoked, has its this context set to the provided value, with a given sequence of arguments preceding any provided when the new function is called.

Key Concepts:
this Context: Refers to the object that the function is currently working with.
Function Invocation: These methods control how functions are invoked and with what context.
Function Borrowing: Using methods of one object on another object by setting the context.

8. Polyfill for Object.assign
Object.assign is a method that copies all enumerable own properties from one or more source objects to a target object. A polyfill for Object.assign would manually iterate over the properties of source objects and copy them to the target object.

Key Concepts:
Shallow Copy: Object.assign performs a shallow copy, meaning it only copies the first level of properties.
Enumerable Properties: Only properties that are enumerable (i.e., not flagged as non-enumerable) are copied.
Target Mutation: The target object is mutated and returned, reflecting the properties copied from the source objects.
These explanations should help you understand the underlying theory and concepts involved in the implementation of the provided coding tasks.

