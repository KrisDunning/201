[Return to Course 201 Notes](https://KrisDunning.github.io/201/)

# Reading 10 - Errors and Debugging

*****

## Bugs in scripts

Order of operations of scripts is one source of bugs in a program. A program may be read from top to bottom but when executed it may jump around the script. Following and understanding the flow of the program may help identify bugs.  

### Execution Context

Every statement in a script lives in one of three execution contexts

- Global Context- Code that is in the script but not in a function. Only one in a page.
- Function Context- Code being run in a function. Each function has its own function context.
- Eval Context(not shown)- Code executed in an internal function called `eval()`

### Variable Scope

The first two execution contexts correspond with the notion of scope.

- Global Scope- If a variable is declared outside a function then it has global scope.
- Function-Level Scope- When a variable is declared within a function it can only be used within that function. This is because it has a function-level scope.

## Execution Context and Hoisting

Each time a script enters a new execution contect there are 2 phases of activity

- Prepare- The new scope is created. Variable, functions and arguments are created. 
- Execute- Now it can assign vales to variable. Reference functions and run their code. Execute Statements.  

Knowing how this process works helps with understanding the concept of ***hoisting***. With hoisting you can call functions before they are decoared. (doesnt work with function expressions). Also allows us to assign value to a variable that has not yet been declared.  

functions are said to have ***lexical scope***. They are linked to the object they were diefined within. If a variables object for the current execution context it can looks in the variables object of the parent execution context. It can affect performance so ideally you create variables inside the finctions that use them.  

Note that you can not access the variables object from code, it is hidden in the interpreter behind the scenes.  

## Errors

JS statements that generate an error throw an `exception` and you can use a `handler` to react to the error.  

There are 7 types of built in error objects

- Error- generic error the others are based on this
- SyntaxError- syntax has not been followed
- ReferenceError- tried to reference a variable not declared or withing scope
- TypeError- Unexpected data type that cannot be coerced
- RangeError- numbers not in acceptable range
- UIError- encodeURI(), decodeURI() and similar methods used incorrectly
- EvalError- eval() function used incorrectly

To deal with errors there are two things to do

- Debug the script to fix errors
- Handle errors gracefully

To debug a common way is to utilize browser dev tools and the javascript console.  

You can also use logging data. The common way is to use the console. console.log(), console.dir(), console.table(), console.info().  

One useful option is the console.assert() method. You can write a test if a condition is met and console.log() of the condition evaluates to false.  

Breakpoints can be used to pause execution of the code and check the values stored at that point in time. If you set multiple breakpoints you can "step through" them one-by-one to see where values change and where a problem might occur. You can even set conditional breakpoints that are triggered when a coondition is met.  

You can create a breakpoint in your code by using the debugger keyword. When dev tools are open this will automatically create a breakpoint.  

### Handling excetions

try, catch, finally  

~~~~JS
try{
  //try to execute this code
} catch(exception){
  //if there is an exception, run this code
} finally {
  //this always gets executed
}
~~~~

You can create your own errors before the interpreter creates them with `throw new Error('message')`  



## Things I want to know more about

Is 3rd party debuggers worth a try? do they offer anything new/useful without paying money

*****