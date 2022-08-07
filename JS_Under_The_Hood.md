#Thread of Execution & the Call Stack

	*[x] JavaScript is a single-threaded language.
	*[x] Single sequential flow of control.
	*[x] JavaScript is a synchromous language with asynchronous capabilities.
	*[x] A thread has a call stack and memory.

								THREAD OF EXECUTION
										|
										|
									Operation 1    { console.log(1); }
										|
										|
									Operation 2    { console.log(2); }
										|
										|
									Operation 3    { console.log(3); }
										|
										|
							Call Stack 		Memory Help



# CALL STACK:

	*[x] Stack of functions to be executed.
	*[x] Manages execution contexts.
	*[x] Stacks are LIFO { last in first out }.


# EXECUTION CONTEXT:

	When we run any JavaScript, a special enviroment is created to handle the transformation & execution of code. This is called Execution context.
	It contains the currently running code and everything that aids in its execution

	There is a global execution context as well as a function execution context for every function invoked.

#Execution Context Phases

	## Memory Creation Phase:

		1. Create the global object ( browser = window, Node.js = global).
		1. Create the 'this' object and bind it to the global object.
		1. Setup memory heap for storing variables and function references.
		1. Store functions and variables in global execution context and set to "undefined".

	## Execution Phase:
		1. Execute code line by line.
		1. Create a new execution context for each function call.
		

