# Applied Visual Design: Create Visual Balance Using the text-align Property

This section of the curriculum focuses on Applied Visual Design. The first group of challenges build on the given card layout to show a number of core principles.

Text is often a large part of web content. CSS has several options for how to align it with the `text-align` property.

`text-align: justify;` causes all lines of text except the last line to meet the left and right edges of the line box.

`text-align: center;` centers the text

`text-align: right;` right-aligns the text

And `text-align: left;` (the default) left-aligns the text.

Align the `h4` tag's text, which says "Google", to the center. Then justify the paragraph tag which contains information about how Google was founded.

# Applied Visual Design: Adjust the Width of an Element Using the width Property
You can specify the width of an element using the width property in CSS. Values can be given in relative length units (such as em), absolute length units (such as px), or as a percentage of its containing parent element. Here's an example that changes the width of an image to 220px:

img {
  width: 220px;
}
Add a width property to the entire card and set it to an absolute value of 245px. Use the fullCard class to select the element.

# Applied Visual Design: Adjust the Height of an Element Using the height Property

You can specify the height of an element using the height property in CSS, similar to the width property. Here's an example that changes the height of an image to 20px:

img {
  height: 20px;
}
Add a height property to the h4 tag and set it to 25px.

Note: You may need to be at 100% zoom to pass the test on this challenge.

# Applied Visual Design: Use the strong Tag to Make Text Bold
To make text bold, you can use the strong tag. This is often used to draw attention to text and symbolize that it is important. With the strong tag, the browser applies the CSS of font-weight: bold; to the element.

Wrap a strong tag around "Stanford University" inside the p tag (do not include the period).

# Applied Visual Design: Use the u Tag to Underline Text

To underline text, you can use the u tag. This is often used to signify that a section of text is important, or something to remember. With the u tag, the browser applies the CSS of text-decoration: underline; to the element.

Wrap the u tag only around the text "Ph.D. students".

Note: Try to avoid using the u tag when it could be confused for a link. Anchor tags also have a default underlined formatting.

# Applied Visual Design: Use the em Tag to Italicize Text
To emphasize text, you can use the em tag. This displays text as italicized, as the browser applies the CSS of font-style: italic; to the element.

Wrap an em tag around the contents of the paragraph tag to give it emphasis.

# Applied Visual Design: Use the s Tag to Strikethrough Text
To strikethrough text, which is when a horizontal line cuts across the characters, you can use the s tag. It shows that a section of text is no longer valid. With the s tag, the browser applies the CSS of text-decoration: line-through; to the element.

Wrap the s tag around "Google" inside the h4 tag and then add the word "Alphabet" beside it, which should not have the strikethrough formatting.

# Applied Visual Design: Create a Horizontal Line Using the hr Element
You can use the hr tag to add a horizontal line across the width of its containing element. This can be used to define a change in topic or to visually separate groups of content.

Add an hr tag underneath the h4 which contains the card title.

Note: In HTML, hr is a self-closing tag, and therefore doesn't need a separate closing tag.

# Applied Visual Design: Adjust the background-color Property of Text
Instead of adjusting your overall background or the color of the text to make the foreground easily readable, you can add a background-color to the element holding the text you want to emphasize. This challenge uses rgba() instead of hex codes or normal rgb().

rgba stands for:
  r = red
  g = green
  b = blue
  a = alpha/level of opacity
The RGB values can range from 0 to 255. The alpha value can range from 1, which is fully opaque or a solid color, to 0, which is fully transparent or clear. rgba() is great to use in this case, as it allows you to adjust the opacity. This means you don't have to completely block out the background.

You'll use background-color: rgba(45, 45, 45, 0.1) for this challenge. It produces a dark gray color that is nearly transparent given the low opacity value of 0.1.

To make the text stand out more, adjust the background-color of the h4 element to the given rgba() value.

Also for the h4, remove the height property and add padding of 10px.

# Applied Visual Design: Adjust the Size of a Header Versus a Paragraph Tag
The font size of header tags (h1 through h6) should generally be larger than the font size of paragraph tags. This makes it easier for the user to visually understand the layout and level of importance of everything on the page. You use the font-size property to adjust the size of the text in an element.

To make the heading significantly larger than the paragraph, change the font-size of the h4 tag to 27 pixels.

# Applied Visual Design: Add a box-shadow to a Card-like Element
The box-shadow property applies one or more shadows to an element.

The box-shadow property takes values for

offset-x (how far to push the shadow horizontally from the element),
offset-y (how far to push the shadow vertically from the element),
blur-radius,
spread-radius and
color, in that order.
The blur-radius and spread-radius values are optional.

Multiple box-shadows can be created by using commas to separate properties of each box-shadow element.

Here's an example of the CSS to create multiple shadows with some blur, at mostly-transparent black colors:

box-shadow: 0 10px 20px rgba(0,0,0,0.19), 0 6px 6px rgba(0,0,0,0.23);
The element now has an id of thumbnail. With this selector, use the example CSS values above to place a box-shadow on the card.

# Applied Visual Design: Decrease the Opacity of an Element
The opacity property in CSS is used to adjust the opacity, or conversely, the transparency for an item.

A value of 1 is opaque, which isn't transparent at all.
A value of 0.5 is half see-through.
A value of 0 is completely transparent.
The value given will apply to the entire element, whether that's an image with some transparency, or the foreground and background colors for a block of text.

Set the opacity of the anchor tags to 0.7 using links class to select them.

# Applied Visual Design: Use the text-transform Property to Make Text Uppercase
The text-transform property in CSS is used to change the appearance of text. It's a convenient way to make sure text on a webpage appears consistently, without having to change the text content of the actual HTML elements.

The following table shows how the different text-transformvalues change the example text "Transform me".

Value	Result
lowercase	"transform me"
uppercase	"TRANSFORM ME"
capitalize	"Transform Me"
initial	Use the default value
inherit	Use the text-transform value from the parent element
none	Default: Use the original text
Transform the text of the h4 to be uppercase using the text-transform property.

# Applied Visual Design: Set the font-size for Multiple Heading Elements
The font-size property is used to specify how large the text is in a given element. This rule can be used for multiple elements to create visual consistency of text on a page. In this challenge, you'll set the values for all h1 through h6 tags to balance the heading sizes.

In the style tags, set the font-size of the:

h1 tag to 68px.
h2 tag to 52px.
h3 tag to 40px.
h4 tag to 32px.
h5 tag to 21px.
h6 tag to 14px.

# Applied Visual Design: Set the font-weight for Multiple Heading Elements

You set the font-size of each heading tag in the last challenge, here you'll adjust the font-weight.

The font-weight property sets how thick or thin characters are in a section of text.

Set the font-weight of the h1 tag to 800.
Set the font-weight of the h2 tag to 600.
Set the font-weight of the h3 tag to 500.
Set the font-weight of the h4 tag to 400.
Set the font-weight of the h5 tag to 300.
Set the font-weight of the h6 tag to 200.

# Applied Visual Design: Set the font-size of Paragraph Text
The font-size property in CSS is not limited to headings, it can be applied to any element containing text.

Change the value of the font-size property for the paragraph to 16px to make it more visible.

# Applied Visual Design: Set the line-height of Paragraphs
CSS offers the line-height property to change the height of each line in a block of text. As the name suggests, it changes the amount of vertical space that each line of text gets.

Add a line-height property to the p tag and set it to 25px.

# Applied Visual Design: Adjust the Hover State of an Anchor Tag
This challenge will touch on the usage of pseudo-classes. A pseudo-class is a keyword that can be added to selectors, in order to select a specific state of the element.

For example, the styling of an anchor tag can be changed for its hover state using the :hover pseudo-class selector. Here's the CSS to change the color of the anchor tag to red during its hover state:

a:hover {
  color: red;
}
The code editor has a CSS rule to style all a tags black. Add a rule so that when the user hovers over the a tag, the color is blue.


# Applied Visual Design: Change an Element's Relative Position

CSS treats each HTML element as its own box, which is usually referred to as the CSS Box Model. Block-level items automatically start on a new line (think headings, paragraphs, and divs) while inline items sit within surrounding content (like images or spans). The default layout of elements in this way is called the normal flow of a document, but CSS offers the position property to override it.

When the position of an element is set to relative, it allows you to specify how CSS should move it relative to its current position in the normal flow of the page. It pairs with the CSS offset properties of left or right, and top or bottom. These say how many pixels, percentages, or ems to move the item away from where it is normally positioned. The following example moves the paragraph 10 pixels away from the bottom:

p {
  position: relative;
  bottom: 10px;
}
Changing an element's position to relative does not remove it from the normal flow - other elements around it still behave as if that item were in its default position. Note: Positioning gives you a lot of flexibility and power over the visual layout of a page. It's good to remember that no matter the position of elements, the underlying HTML markup should be organized and make sense when read from top to bottom. This is how users with visual impairments (who rely on assistive devices like screen readers) access your content.

Change the position of the h2 to relative, and use a CSS offset to move it 15 pixels away from the top of where it sits in the normal flow. Notice there is no impact on the positions of the surrounding h1 and p elements.

# Applied Visual Design: Move a Relatively Positioned Element with CSS Offsets
The CSS offsets of top or bottom, and left or right tell the browser how far to offset an item relative to where it would sit in the normal flow of the document. You're offsetting an element away from a given spot, which moves the element away from the referenced side (effectively, the opposite direction). As you saw in the last challenge, using the top offset moved the h2 downwards. Likewise, using a left offset moves an item to the right.



Use CSS offsets to move the h2 15 pixels to the right and 10 pixels up.

# Applied Visual Design: Lock an Element to its Parent with Absolute Positioning

The next option for the CSS position property is absolute, which locks the element in place relative to its parent container. Unlike the relative position, this removes the element from the normal flow of the document, so surrounding items ignore it. The CSS offset properties (top or bottom and left or right) are used to adjust the position.

One nuance with absolute positioning is that it will be locked relative to its closest positioned ancestor. If you forget to add a position rule to the parent item, (this is typically done using position: relative;), the browser will keep looking up the chain and ultimately default to the body tag.

Lock the #searchbar element to the top-right of its section parent by declaring its position as absolute. Give it top and right offsets of 50 pixels each.

# Applied Visual Design: Lock an Element to the Browser Window with Fixed Positioning
The next layout scheme that CSS offers is the fixed position, which is a type of absolute positioning that locks an element relative to the browser window. Similar to absolute positioning, it's used with the CSS offset properties and also removes the element from the normal flow of the document. Other items no longer "realize" where it is positioned, which may require some layout adjustments elsewhere.

One key difference between the fixed and absolute positions is that an element with a fixed position won't move when the user scrolls.

The navigation bar in the code is labeled with an id of navbar. Change its position to fixed, and offset it 0 pixels from the top and 0 pixels from the left. After you have added the code, scroll the preview window to see how the navigation stays in place.

