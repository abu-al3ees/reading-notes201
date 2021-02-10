<img> images.html HTML
To add an image into the page
you need to use an <img>
element. This is an empty
element (which means there is
no closing tag). It must carry the
following two attributes:
src
This tells the browser where
it can find the image file. This
will usually be a relative URL
pointing to an image on your
own site. (Here you can see that
the images are in a child folder
called images — relative URLs
were covered on pages 83-84).
alt
This provides a text description
of the image which describes the
image if you cannot see it.

### height
This specifies the height of the
image in pixels.
### width
This specifies the width of the
image in pixels.
### align 
The align attribute was
commonly used to indicate how
the other parts of a page should
flow around an image. It has
been removed from HTML5
and new websites should use
CSS to control the alignment of
images

- The <img> element is used to add images to a
web page.
- You must always specify a src attribute to indicate the
source of an image and an alt attribute to describe the
content of an image.
-  You should save images at the size you will be using
them on the web page and in the appropriate format.
-  Photographs are best saved as JPEGs; illustrations or
logos that use flat colors are better saved as GIFs.

The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:
rgb values
These express colors in terms
of how much red, green and
blue are used to make it up. For
example: rgb(100,100,90)
hex codes
These are six-digit codes that
represent the amount of red,
green and blue in a color,
preceded by a pound or hash #
sign. For example: #ee3e80
color names
There are 147 predefined color
names that are recognized
by browsers. For example:
DarkCya

## RGB Values
Values for red, green, and blue
are expressed as numbers
between 0 and 255.

## Hex Codes
Hex values represent values
for red, green, and blue in
hexadecimal code.

## Color Names
Colors are represented by
predefined names. However,
they are very limited in number

### hue
Hue is the colloquial idea of
color. In HSL colors, hue is often
represented as a color circle
where the angle represents the
color, although it may also be
shown as a slider with values
from 0 to 360.

### saturation
Saturation is the amount of
gray in a color. Saturation is
represented as a percentage.
100% is full saturation and 0%
is a shade of gray.

### lightness
Lightness is the amount of
white (lightness) or black
(darkness) in a color. Lightness
is represented as a percentage.
0% lightness is black, 100%
lightness is white, and 50%
lightness is normal. Lightness
is sometimes referred to as
luminosity.


- Color not only brings your s XX ite to life, but also helps
convey the mood and evokes reactions.
- There are three ways to specify colors in CSS:
RGB values, hex codes, and color names.
- Color pickers can help you find the color you want.
- It is important to ensure that there is enough contrast
between any text and the background color (otherwise
people will not be able to read your content).
- CSS3 has introduced an extra value for RGB colors to
indicate opacity. It is known as RGBA.
- CSS3 also allows you to specify colors as HSL values,
with an optional opacity value. It is known as HSLA.

### Serif
Serif fonts have extra details on
the ends of the main strokes of
the letters. These details are
known as serifs.

### Sans-Serif
Sans-serif fonts have straight
ends to letters, and therefore
have a much cleaner design.

### Monospace
Every letter in a monospace (or
fixed-width) font is the same
width. (Non-monospace fonts
have different widths.)

Setting font size in pixels is the
best way to ensure that the type
appears at the size you intended
(because percentages and ems
are more likely to vary if a user
has changed the default size of
text in their browser).
Pixels are relative to the
resolution of the screen, so the
same type size will look larger
when a screen has a resolution
of 800x600 than it would when
it is 1280x800.
You can also use pt for point
sizes instead of px for pixels, but
you should only do this when
creating style sheets for printerfriendly
versions of pages.
The default size of text in a
web browser is 16 pixels. Using
percentages of this amount, you
can create a scale where the
default text size is 12 pixels, and
headings are sized in relation
to this.
It is possible for users to change
the default size of text in their
web browsers. If they have
done this, the fonts will be
displayed at the same scale that
the designer intended, but at a
larger size.
Ems allow you to change the size
of text relative to the size of the
text in the parent element. Since
the default size of text in web
browsers is 16 pixels, you can
use similar rules to those shown
for percentages.
Because users can change
the default size of text in their
browser, the fonts could all
appear larger (or smaller) than
the designer intended.
The extra p rule above is to help
Internet Explorer 6 and 7 display
the fonts at the right size.
Without this extra rule, IE6 and
IE7 exaggerate the relative sizes
of other text.
:hover
This is applied when a user
hovers over an element with a
pointing device such as a mouse.
This has commonly been used
to change the appearance of
links and buttons when a user
places their cursor over them. It
is worth noting that such events
do not work on devices that use
touch screens (such as the iPad)
because the screen is not able to
tell when someone is hovering
their finger over an element.
:active
This is applied when an element
is being activated by a user; for
example, when a button is being
pressed or a link being clicked.
Sometimes this is used to make
a button or link feel more like it
is being pressed by changing the
style or position of the element
slightly.
:focus
This is applied when an element
has focus. Any element that
you can interact with, such as a
link you can click on or any form
control can have focus.

- There are properties to control t XX he choice of font, size,
weight, style, and spacing.
- There is a limited choice of fonts that you can assume
most people will have installed.
-  If you want to use a wider range of typefaces there are
several options, but you need to have the right license
to use them.
-  You can control the space between lines of text,
individual letters, and words. Text can also be aligned
to the left, right, center, or justified. It can also be
indented.
-  You can use pseudo-classes to change the style of an
element when a user hovers over or clicks on text, or
when they have visited a link.




















