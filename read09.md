## Form Controls
ADDING TEXT:
Ma king Choice s:
Submitting Forms: Uploadi ng Files:
### Password input
Like a single line text box but it
masks the characters entered.
Text input (single-line)
Used for a single line of text such
as email addresses and names.
### Text area (multi-line)
For longer areas of text, such as
messages and comments.

How Forms Work
Thank you, Ivy!
You voted for Herbie Hancock.
A user fills in a form and then presses a button
to submit the information to the server.

A form may have several form controls, each
gathering different information. The server
needs to know which piece of inputted data
corresponds with which form element

<form>
Form controls live inside a
<form> element. This element
should always carry the action
attribute and will usually have a
method and id attribute too.
action
Every <form> element requires
an action attribute. Its value
is the URL for the page on the
server that will receive the
information in the form when it
is submitted.
method
Forms can be sent using one of
two methods: get or post.

<input>
The <input> element is used
to create several different form
controls. The value of the type
attribute determines what kind
of input they will be creating

<textarea>
The <textarea> element
is used to create a mutli-line
text input. Unlike other input
elements this is not an empty
element. It should therefore have
an opening and a closing tag.

<select>
A drop down list box (also
known as a select box) allows
users to select one option from a
drop down list.

<button>
The <button> element was
introduced to allow users more
control over how their buttons
appear, and to allow other
elements to appear inside the
button.

- In addition to the CSS p XX roperties covered in other
chapters which work with the contents of all elements,
there are several others that are specifically used to
control the appearance of lists, tables, and forms.
- List markers can be given different appearances
using the list-style-type and list-style image
properties.
-  Table cells can have different borders and spacing in
different browsers, but there are properties you can
use to control them and make them more consistent.
- Forms are easier to use if the form controls are
vertically aligned using CSS.
- Forms benefit from styles that make them feel more
interactive.

The browser represents the page using a DOM tree.
DOM trees have four types of nodes: document nodes,
element nodes, attribute nodes, and text nodes.
You can select element nodes by their id or cl ass
attributes, by tag name, or using CSS selector syntax.
Whenever a DOM query can return more than one
node, it will always return a Nadel i st.
From an element node, you can access and update its
content using properties such as textContent and
i nnerHTML or using DOM manipulation techniques.
An element node can contain multiple text nodes and
child elements that are siblings of each other.
In older browsers, implementation of the DOM is
inconsistent (and is a popular reason for using jQuery).
Browsers offer tools for viewing the DOM tree


- SELECT ELEMENT
The element that users are
interacting with is the text input
where they enter the username.

When an event occurs, the event object tells
you information about the event, and the
element it happened upon.

Every time an event fires, the The event object is passed to
event object contains helpful any function that is the event
data about the event, such as: handler or listener.
• Which element the event
happened on If you need to pass arguments
• Which key was pressed for a to a named function, the event
keypress event object will first be passed to the
• What part of the viewport the anonymous wrapper function
user clicked for a c 1 i ck event (this happens automatically);
(the viewport is the part of then you must specify it as a
the browser window that parameter of the named function
shows the web page) (as shown on the next page).

## EVENT DELEGATION
Creating event listeners for a lot of elements
can slow down a page, but event flow allows
you to listen for an event on a parent element.

preventDef au 1t ()
Some events, such as clicking on
links and submitting forms, take
the user to another page

stopPropagation()
Once you have handled an
event using one element, you
may want to stop that event
from bubbling up to its ancestor
elements (especially if there
are separate event handlers
responding to the same events
on the containing elements).

USING BOTH METHODS
You will sometimes see the
following used in similar
situations that are in a function:
r eturn false;

