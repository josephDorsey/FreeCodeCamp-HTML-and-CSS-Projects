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

