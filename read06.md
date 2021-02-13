some function return information to the code that called them
- function can return more than one value using array
FUNCTION DECLARATION
A function declaration creates a function that you
can ca ll later in your code. It is the type of function
you have seen so far in this book.

FUNCTION EXPRESSION
If you put a function where the interpreter would
expect to see an expression, then it is treated as an
expression, and it is known as a function expression.
In function expressions, the name is usually omitted.

LOCAL VARIABLES
When a variable is created inside a function using the
var keyword, it can only be used in that function.
It is called a local variable or function-level variable.
It is said to have local scope or function-level scope.
It cannot be accessed outside of the function in
which it was declared. Below, area is a local variable.

GLOBAL VARIABLES
If you create a variable outside of a function, then it
can be used anywhere within the script. It is called a
global variable and has global scope. In the example
shown, wa 11 Size is a global variable

Conditional statements allow your code to make
decisions about what to do next.
Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>)
are used to compare two operands.
Logical operators allow you to combine more than one
set of comparison operators.
if ... else statements allow you to run one set of code
if a condition is true, and another if it is false.
switch statements allow you to compare a value
against possible outcomes (and also provides a default
option if none match).
Data types can be coerced from one type to another.
All values evaluate to either truthy or falsy.
There are three types of loop: for, while, and
do ... while. Each repeats a set of statements

## The Document Object Model (DOM) specifies
how browsers should create a model of an HTML
page and how JavaScript can access and update the
contents of a web page while it is in the browser window.

DOM queries may return one element, or they may return a Nodelist,
which is a collection of nodes.
Sometimes you will just want to access one
individual element (or a fragment of the page that
is stored within that one element). Other times you
may want to select a group of element s, for example,
every <hl> element in the page or every <1 i>
element within a particular list.
Here, the DOM tree shows the body of the page of
the list example. We focus on accessing elements
first so it only shows element nodes. The diagrams
in the coming pages highlight which elements a
DOM query would return. (Remember, element
nodes are the DOM representation of an element.)


get El ementByid () al lows you
to select a single element node
by specifying the value of its
id attribute.

The get El ementsByCl ass Name()
method allows you to select
elements whose c 1 ass attribute
contains a specific va lue.

The get El ementsByTagName ()
method allows you to select
elements using their tag name.

querySe 1 ector() returns
the first element node that
matches the CSS-style selector.
querySe 1ectorA11 () returns a
Nodelist of all of the matches.

parentNode
This property finds the element
node for the containing (or
parent) element in the HTML.

previousSibling
nextSibling
These properties find the
previous or next sibling of a node
if there are siblings.

firstChild
lastChild
These properties find the first or
last child of the current element.

ACCESS & UPDATE TEXT &
MARKUP WITH INNERHTML

innerHTML
When getting HTML from an
element, the i nnerHTML property
will get the content of an
element and return it as one long
string, including any markup that
the element contains.

createEl ement ()
You start by creating a new
element node using the
createElement() method.
This element node is stored
in a variable.

createTextNode() allows you to
create a new text node to attach
to an element. It is stored in a
variable called newText

appendChi 1 d () is used
again - this time to insert the
new element and its content into
the DOM tree.

























