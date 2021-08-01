Html book
chapter 5:
images:
Images can be used to set the tone for a site in less time than it takes to read a description because of that:

Be relevant
Convey information
Convey the right mood
Be instantly recognisable
Fit the color palett
Adding Images To add an image into the page you need to use an  element. This is an empty element (which means there is no closing tag). It must carry the following two attributes:

src This tells the browser where it can find the image file
alt This provides a text description of the image which describes the image if you cannot see it
title You can also use the title attribute with the  element to provide additional information about the image

You will also often see an  element use two other attributes that specify its size: 1 height This specifies the height of the image in pixels. 2. width This specifies the width of the image in pixels.

Inline elements sit within a block level element and do not start on a new line

The align attribute was commonly used to indicate how the other parts of a page should flow around an image.

The align attribute can take these horizontal values:

left
right
Three Rules for Creating Images:

Save images in the right format
Save images at the right size
Use the correct resolution
Creating an image that is partially transparent (or "see-through") for the web involves selecting one of two formats:

Transparent GIF
PNG
note:Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.

Chapter 11 :
Color not only brings your site to life, but also helps convey the mood and evokes reactions.

Foreground Color :The color property allows you to specify the color of text inside an element

rgb values; rgb(102,205,170)
hex codes;#66cdaa
color names;MediumAquaMarine
Every color on a computer screen is created by mixing amounts of red,green, and blue. To find the color you want, you can use a color picker.

Hue: is near to the colloquial idea of color. Technically speaking however, a color can also have saturation and brightness as well as hue.

Saturation: refers to the amount of gray in a color. At maximum saturation, there would be nogray in the color. At minimum saturation, the color would be mostly gray.

Brightness: (or "value") refersto how much black is in a color. At maximum brightness, there would be no black in the color.At minimum brightness, the color would be very dark.

The hsl color property has been introduced in CSS3 as an alternative way to specify colors.

Chapter12
The properties that allow you to controlthe appearance of text can be split into two groups:

Those that directly affect the font and its appearance(including the typeface, whether it is regular, bold or italic,and the size of the text)
Those that would have the same effect on text no matter what font you were using (including the color of text andthe spacing between words and letters)
Typeface :

Serif: Serif fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs.
Sans-Serif:sans-serif fonts have straight ends to letters, and therefore have a much cleaner design.
Monospace:every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fontshave different widths.)
*When choosinga typeface, it is important to understand that a browser will usually only display it if it'sinstalled on that user's computer

Bold font-weight

normal:This causes text to appear at a normal weight.
bold:This causes text to appear bold.
Styling Links :link, This allows you to set styles for links that have not yet been visited :visited This allows you to set styles for links that have been clicked on.

:hover This is applied when a user hovers over an element with a pointing device such as a mouse. This has commonly been used to change the appearance of links and buttons when a user places their cursor over them

:active This is applied when an element is being activated by a user; for example, when a button is being pressed or a link being clicked

:focus This is applied when an element has focus. Any element that you can interact with, such as a link you can click on or any form control can have focus.

Attribute Selectors
Existence []Matches a specific attribute,p[class]
Equality [=] Matches a specific attribute with a specific value,p[class="dog"]
Space [=] Matches a specific attribute whose value appears in a spaceseparated list of words,p[class="dog"]
Prefix[^=] Matches a specific attribute whose value begins with a specific string,p[attr^"d"]
SubString[=] Matches a specific attribute whose value contains a specific substring,p[attr"do"]
Suffix [$=] Matches a specific attribute whose value ends with a specific string p[attr$"g"]
There is a limited choice of fonts that you can assume most people will have installed.

You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link.