# The stack: Javascript interperter processes one line of a code at a time ,when the code have a function it stacks the function and then complete the code .

## UNDERSTANDING ERRORS
If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handling code

### Syntax Error
SYNTAX IS NOT CORRECT
This is caused by incorrect use of the rules of the
language. It is often the result of a simple typo.

### Reference Error
VARIABLE DOES NOT EXIST
This is caused by a variable that is not declared or is
out of scope

- Error
GENERIC ERROR OBJECT
The generic Error object is the template (or
prototype) from which all other error objects are
created

- NaN
NOT AN ERROR
Note: If you perform a mathematical operation using
a value that is not a number, you end up with the
value of NaN, not a type error.


1: DEBUG THE SCRIPT TO FIX ERRORS
If you come across an error while writing a script
(or when someone reports a bug), you will need to
debug the code, track down the source of the error,
and fix it.

2: HANDLE ERRORS GRACEFULLY
You can handle errors gracefully using try, catch,
throw, and f i na 1 ly statements.

The JavaScript console will tell you when there is a problem with a script,
where to look for the problem, and what kind of issue it seems to be


If you understand execution contexts (which have two
stages) and stacks, you are more likely to find the error
in your code.
Debugging is the process of finding errors. It involves a
process of deduction.
The console helps narrow down the area in which the
error is located, so you can try to find the exact error.
JavaScript has 7 different types of errors. Each creates
its own error object, which can tell you its line number
and gives a description of the error.
If you know that you may get an error, you can handle
it gracefully using the try, catch, finally statements.
Use them to give your users helpful feedback.