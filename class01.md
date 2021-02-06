# Structuring Word
# Documents

The use of headings and
subheadings in any document
often reflects a hierarchy of
information. For example, a
document might start with
a large heading, followed by
an introduction or the most
important information.
This might be expanded upon
under subheadings lower down
on the page. When using a word
processor to create a document,
we separate out the text to give
it structure. Each topic might
have a new paragraph, and each
section can have a heading to
describe what it covers.
On the right, you can see a
simple document in Microsoft
Word. The different styles for
the document, such as different
levels of heading, are shown
in the drop down box. If you
regularly use Word, you might
have also used the formatting
toolbar or palette to do this.
# HTM L Describes
# the Structure
# of Pages
In the browser window you can see a web page that features exactly
the same content as the Word document you met on the page 18. To
describe the structure of a web page, we add code to the words we want
to appear on the page.
You can see the HTML code for this page below. Don't worry about what
the code means yet. We start to look at it in more detail on the next
page. Note that the HTML code is in blue, and the text you see on screen
is in black.
<html>
<body>
<h1>This is the Main Heading</h1>
<p>This text might be an introduction to the rest of
the page. And if the page is a long one it might
be split up into several sub-headings.<p>
<h2>This is a Sub-Heading</h2>
<p>Many long articles have sub-headings so to help
you follow the structure of what is being written.
There may even be sub-sub-headings (or lower-level
headings).</p>
<h2>Another Sub-Heading</h2>
<p>Here you can see another sub-heading.</p>
</body>
</html>
The HTML code (in blue) is made up of characters that live inside angled
brackets — these are called HTML elements. Elements are usually
made up of two tags: an opening tag and a closing tag. (The closing tag
has an extra forward slash in it.) Each HTML element tells the browser
something about the information that sits between its opening and
closing tags.

# Body, Head & Title
## <body>
You met the <body> element
in the first example we created.
Everything inside this element is
shown inside the main browser
window.
## <head>
Before the <body> element you
will often see a <head> element.
This contains information
about the page (rather than
information that is shown within
the main part of the browser
window that is highlighted in
blue on the opposite page).
You will usually find a <title>
element inside the <head>
element.
## <title>
The contents of the <title>
element are either shown in the
top of the browser, above where
you usually type in the URL of
the page you want to visit, or
on the tab for that page (if your
browser uses tabs to allow you
to view multiple pages at the
same time).

## DOCTYPEs
Because there have been
several versions of HTML, each
web page should begin with a
DOCTYPE declaration to tell a
browser which version of HTML
the page is using (although
browsers usually display the
page even if it is not included).
We will therefore be including
one in each example for the rest
of the book.
As you will see when we come to
look at CSS and its box model on
page 316, the use of a DOCTYPE
can also help the browser to
render a page correctly.
Because XHTML was written
in XML, you will sometimes
see pages that use the XHTML
strict DOCTYPE start with
the optional XML declaration.
Where this is used, it should be
the first thing in a document.
There must be nothing before it,
not even a space.

## Comments in HTML
## <!-- -->
If you want to add a comment
to your code that will not be
visible in the user's browser, you
can add the text between these
characters:
<!-- comment goes here -->
It is a good idea to add
comments to your code because,
no matter how familiar you
are with the page at the time
of writing it, when you come
back to it later (or if someone
else needs to look at the code),
comments will make it much
easier to understand.
Although comments are not
visible to users in the main
browser window, they can be
viewed by anyone who looks at
the source code behind the page.
On a long page you will often
see comments used to indicate
where sections of the page start
or end, and to pass on notes to
help anyone who is looking at
the code understand it.
Comments can also be used
around blocks of code to stop
that code from being displayed
in the browser. In the example on
the left, the email link has been
commented out.

# ID Attribute
Every HTML element can carry
the id attribute. It is used to
uniquely identify that element
from other elements on the
page. Its value should start with
a letter or an underscore (not a
number or any other character).
It is important that no two
elements on the same page
have the same value for their id
attributes (otherwise the value is
no longer unique).
As you will see when you
come to look at CSS in the next
section, giving an element a
unique identity allows you to
style it differently than any other
instance of the same element
on the page. For example,
you might want to assign one
paragraph within the page
(perhaps a paragraph containing
a pull quote) a different style
than all of the other paragraphs.
In the example on the right, the
paragraph with the id attribute
whose value is pullquote is
made uppercase using CSS.
If you go on to learn about
JavaScript (a language that
allows you to add interactivity to
your pages), id attributes can be
used to allow the script to work
with that particular element.
The id attribute is known as a
global attribute because it can
be used on any element.

# Class Attribute
Every HTML element can
also carry a class attribute.
Sometimes, rather than uniquely
identifying one element within
a document, you will want a
way to identify several elements
as being different from the
other elements on the page.
For example, you might have
some paragraphs of text that
contain information that is more
important than others and want
to distinguish these elements, or
you might want to differentiate
between links that point to other
pages on your own site and links
that point to external sites.
To do this you can use the
class attribute. Its value
should describe the class it
belongs to. In the example on
the left, key paragraphs have a
class attribute whose value is
important.
The class attribute on any
element can share the same
value. So, in this example, the
value of important could be
used on headings and links, too.
Result
<p class="important">For a one-year period from
November 2010, the Marugame Genichiro-Inokuma
Museum of Contemporary Art (MIMOCA) will host a
cycle of four Hiroshi Sugimoto exhibitions.</p>
<p>Each will showcase works by the artist
thematically contextualized under the headings
"Science," "Architecture," "History" and
"Religion" so as to present a comprehensive
panorama of the artist's oeuvre.</p>
<p class="important admittance">Hours: 10:00 – 18:00
(No admittance after 17:30)</p>
HTML chapter-08/class-attribute.html
Class Attribute
By default, using these attributes
does not affect the presentation
of an element. It will only change
their appearance if there is a CSS
rule that indicates it should be
displayed differently.
In this example, CSS has been
applied to make elements with
a class attribute whose value
is important uppercase, and
elements with a class attribute
whose value is admittance red.
If you would like to indicate that
an element belongs to several
classes, you can separate class
names with a space, as you can
see in the third paragraph in the
example above.

# Grouping Text &
# Elements In a Block
<div> block-elements.html HTML
The <div> element allows you to
group a set of elements together
in one block-level box.
For example, you might create
a <div> element to contain all
of the elements for the header
of your site (the logo and the
navigation), or you might create
a <div> element to contain
comments from visitors.
In a browser, the contents of
the <div> element will start on
a new line, but other than this
it will make no difference to the
presentation of the page.
Using an id or class attribute
on the <div> element, however,
means that you can create
CSS style rules to indicate how
much space the <div> element
should occupy on the screen and
change the appearance of all the
elements contained within it.
It can also make it easier to
follow your code if you have used
<div> elements to hold each
section of the page.
Grouping Te xt &
Eleme nts In a Block
Since there may be several
other elements inside a <div>
element, it can be helpful to add
a comment after the closing
</div> tag.
This allows you to clearly see
which opening tag it is supposed
to correspond to, as shown at
the end of the example here.

# Grouping Te xt &
# Elements Inline
 ## <span>
The <span> element acts like
an inline equivalent of the <div>
element. It is used to either:
1. Contain a section of text
where there is no other suitable
element to differentiate it from
its surrounding text
2. Contain a number of inline
elements
The most common reason why
people use <span> elements
is so that they can control the
appearance of the content of
these elements using CSS.
You will usually see that a class
or id attribute is used with
<span> elements:
●● To explain the purpose of this
<span> element
●● So that CSS styles can be
applied to elements that
have specific values for these
attributes.

# Headers & Footers
<header> <footer>
The <header> and <footer>
elements can be used for:
●● The main header or footer
that appears at the top or
bottom of every page on the
site.
●● A header or footer for an
individual <article> or
<section> within the page.
In this example, the <header>
element used to contain the site
name and the main navigation.
The <footer> element contains
copyright information, along
with links to the privacy policy
and terms and conditions.
Each individual <article> and
<section> element can also
have its own <header> and
<footer> elements to hold the
header or footer information for
that section within the page.
For example, on a page with
several blog posts, each
individual post can be thought
of as a separate section. The
<header> element can therefore
be used to contain the title and
date of each individual post, and
the <footer> might contain
links to share the article on
social networking sites.
Please note that all of the
code shown in this chapter
is referenced in one HTML
document which is called:
html5-layout.html
Headers & Footers
<header> <footer>
<footer>
&copy; 2011 Yoko's Kitchen
</footer>

# Articles
# <article>

The <article> element acts as
a container for any section of a
page that could stand alone and
potentially be syndicated.
This could be an individual
article or blog entry, a comment
or forum post, or any other
independent piece of content.
If a page contains several articles
(or even summaries of several
articles), then each individual
article would live inside its own
<article> element.
The <article> elements can
even be nested inside each
other. For example, a blog post
might live inside one <article>
element and each comment on
the article could live inside its
own child <article> element.

# Who is the Site For?

Every website should be designed for the
target audience—not just for yourself or the
site owner. It is therefore very important to
understand who your target audience is.
Who is the Site For?
Target Audience: individuals
What is the age range o ●● f your target audience?
●● Will your site appeal to more women or men? What is the mix?
●● Which country do your visitors live in?
●● Do they live in urban or rural areas?
●● What is the average income of visitors?
●● What level of education do they have?
●● What is their marital or family status?
●● What is their occupation?
●● How many hours do they work per week?
●● How often do they use the web?
●● What kind of device do they use to access the web?
Target Audience: Companies
●● What is the size of the company or relevant department?
●● What is the position of people in the company who visit your site?
●● Will visitors be using the site for themselves or for someone else?
●● How large is the budget they control?
It can be helpful to ask some
questions about the people you
would expect to be interested in
the subject of your site.
If you ask a client who a site is
for, it is not uncommon for them
to answer "the entire world."
Realistically, it is unlikely to be
relevant to everyone. If your site
sells light bulbs, even though
most people using a computer
probably use light bulbs, they
are not likely to order them from
someone in a different country.
Even if the site has a wide
appeal, you can still think about
the demographics of a sample of
the target audience.

# What Information
# Your Visitors Need
You know who is coming to your site and why
they are coming, so now you need to work out
what information they need in order to achieve
their goals quickly and effectively.
You may want to offer additional
supporting information that you
think they might find helpful.
Look at each of the reasons why
people will be visiting your site
and determine what they need to
achieve their goals.
You can prioritize levels of
information from key points
down to non-essential or
background information.
By ensuring that you provide the
information that your visitors
are looking for, they will consider
your site more relevant to them.
Therefore, you will have more
opportunity to tell them any
extra information that you think
would be helpful to them (or to
expose them to other products
and services you want to
promote).
If you do not appear relevant to
them by answering their needs,
however, they are likely to go
elsewhere.
Here are some questions to help
you decide what information to
provide for visitors to your site...
Key Information
Will v ●● isitors be familiar with
your subject area / brand
or do you need to introduce
yourself?
●● Will they be familiar with
the product / service /
information you are covering
or do they need background
information on it?
●● What are the most important
features of what you are
offering?
●● What is special about what
you offer that differentiates
you from other sites that offer
something similar?
●● Once people have achieved
the goal that sent them to
your site, are there common
questions people ask about
this subject area?

# Site Maps
Now that you know what needs to appear
on your site, you can start to organize the
information into sections or pages.
The aim is to create a diagram
of the pages that will be used
to structure the site. This is
known as a site map and it will
show how those pages can be
grouped.
To help you decide what
information should go on each
page, you can use a technique
called card sorting.
This involves placing each
piece of information that a
visitor might need to know on
a separate piece of paper and
then organizing the related
information into groups.
Each group relates to a page and,
on larger sites the, pages can in
turn can be grouped together to
create different sections of the
website.
The groups of information are
then turned into the diagram
that is known as the site map.
Sometimes it can be helpful to
ask people who are the target
audience to help you group
related information together.
A site map will usually
begin with the homepage.
Additionally, if the site is large
and is compartmentalized
into sections, each section
might require its own section
homepage to link to all of the
information within it.
For example, most online shops
have section homepages for
each type of product, which then
in turn link to individual product
pages.
You may need to duplicate some
information if it needs to appear
on more than one page.
The pages (or groups of pages)
will inform how users navigate
through the site.
Remember to focus on the
goals that your visitors want to
achieve.
It is worth noting that the
site owner might organize
information in a way that is
different to what the public
expects. It is important to reflect
the public's understanding of the
subject (rather than just the site
owner's understanding of it).
# EVENTS
In the real world, people interact with objects. These interactions can
change the values of the properties in these objects.

WHAT IS AN EVENT?
There are common ways in which people interact
with each type of object. For example, in a car a
driver will typically use at least two pedals. The car
has been designed to respond differently when the
driver interacts with each of the different pedals:
• The accelerator makes the car go faster
• The brake slows it down
Similarly, programs are designed to do different
things when users interact with the computer in
different ways. For example, clicking on a contact
link on a web page could bring up a contact
form, and entering text into a search box may
automatically trigger the search functionality.
An event is the computer's way of sticking up its
hand to say, "Hey, this just happened!"
@ THE ABC OF PROGRAMMING
WHAT DOES AN EVENT DO?
Programmers choose which events they respond to.
When a specific event happens, that event can be
used to trigger a specific section of the code.
Scripts often use different events to trigger different
types of functionality.
So a script will state which events the programmer
wants to respond to, and what part of the script
should be run when each of those events occur

















































































