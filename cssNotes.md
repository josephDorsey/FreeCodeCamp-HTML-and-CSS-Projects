# Introduction to Basic CSS
`Cascading Style Sheets (CSS)` tell the browser how to display the text and other content that you write in HTML.

Note that `CSS` is case-sensitive so be careful with your capitalization.

`CSS` has been adopted by all major browsers and allows you to control:

color
fonts
positioning
spacing
sizing
decorations
transitions

There are *three main ways to apply CSS styling.* You can apply inline styles directly to HTML elements with the style attribute. Alternatively, you can place CSS rules within style tags in an HTML document. Finally, you can write CSS rules in an external style sheet, then reference that file in the HTML document. Even though the first two options have their use cases, most developers prefer external style sheets because they keep the styles separate from the HTML elements. This improves the readability and reusability of your code.

The idea behind CSS is that you can use a selector to target an HTML element in the DOM (Document Object Model) and then apply a variety of attributes to that element to change the way it is displayed on the page.

In this section, you'll see how adding CSS styles to the elements of your CatPhotoApp can change it from simple text to something more.

# Basic CSS: Change the Color of Text
Now let's change the color of some of our text.

We can do this by changing the style of your h2 element.

The property that is responsible for the color of an element's text is the color style property.

Here's how you would set your h2 element's text color to blue:

<h2 style="color: blue;">CatPhotoApp</h2>

Note that it is a good practice to end inline style declarations with a ; .

Change your h2 element's style so that its text color is red.

# Basic CSS: Use a CSS Class to Style an Element
Classes are reusable styles that can be added to HTML elements.

Here's an example CSS class declaration:

<style>
  .blue-text {
    color: blue;
  }
</style>

You can see that we've created a CSS class called blue-text within the <style> tag. You can apply a class to an HTML element like this: <h2 class="blue-text">CatPhotoApp</h2> Note that in your CSS style element, class names start with a period. In your HTML elements' class attribute, the class name does not include the period.

Inside your style element, change the h2 selector to .red-text and update the color's value from blue to red.

Give your h2 element the class attribute with a value of 'red-text'.

# Basic CSS: Style Multiple Elements with a CSS Class
Classes allow you to use the same CSS styles on multiple HTML elements. You can see this by applying your red-text class to the first p element.

# Basic CSS: Change the Font Size of an Element
Font size is controlled by the font-size CSS property, like this:

h1 {
  font-size: 30px;
}
Inside the same <style> tag that contains your red-text class, create an entry for p elements and set the font-size to 16 pixels (16px).


# Basic CSS: Set the Font Family of an Element
You can set which font an element should use, by using the font-family property.

For example, if you wanted to set your h2 element's font to sans-serif, you would use the following CSS:

h2 {
  font-family: sans-serif;
}

# Basic CSS: Import a Google Font

In addition to specifying common fonts that are found on most operating systems, we can also specify non-standard, custom web fonts for use on our website. There are many sources for web fonts on the Internet. For this example we will focus on the Google Fonts library.

Google Fonts is a free library of web fonts that you can use in your CSS by referencing the font's URL.

So, let's go ahead and import and apply a Google font (note that if Google is blocked in your country, you will need to skip this challenge).

To import a Google Font, you can copy the font's URL from the Google Fonts library and then paste it in your HTML. For this challenge, we'll import the Lobster font. To do this, copy the following code snippet and paste it into the top of your code editor (before the opening style element):

<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">

Now you can use the Lobster font in your CSS by using Lobster as the FAMILY_NAME as in the following example:
font-family: FAMILY_NAME, GENERIC_NAME;.

The GENERIC_NAME is optional, and is a fallback font in case the other specified font is not available. This is covered in the next challenge.

Family names are case-sensitive and need to be wrapped in quotes if there is a space in the name. For example, you need quotes to use the "Open Sans" font, but not to use the Lobster font.

Import the Lobster font to your web page. Then, use an element selector to set Lobster as the font-family for your h2 element.

# Basic CSS: Specify How Fonts Should Degrade
There are several default fonts that are available in all browsers. These generic font families include monospace, serif and sans-serif

When one font isn't available, you can tell the browser to "degrade" to another font.

For example, if you wanted an element to use the Helvetica font, but degrade to the sans-serif font when Helvetica isn't available, you will specify it as follows:

p {
  font-family: Helvetica, sans-serif;
}

Generic font family names are not case-sensitive. Also, they do not need quotes because they are CSS keywords.

To begin, apply the monospace font to the h2 element, so that it now has two fonts - Lobster and monospace.

In the last challenge, you imported the Lobster font using the link tag. Now comment out that import of the Lobster font (using the HTML comments you learned before) from Google Fonts so that it isn't available anymore. Notice how your h2 element degrades to the monospace font.

Note: If you have the Lobster font installed on your computer, you won't see the degradation because your browser is able to find the font.

# Basic CSS: Size Your Images
CSS has a property called width that controls an element's width. Just like with fonts, we'll use px (pixels) to specify the image's width.

For example, if we wanted to create a CSS class called larger-image that gave HTML elements a width of 500 pixels, we'd use:

<style>
  .larger-image {
    width: 500px;
  }
</style>
Create a class called smaller-image and use it to resize the image so that it's only 100 pixels wide.

# Basic CSS: Add Borders Around Your Elements
CSS borders have properties like style, color and width.

For example, if we wanted to create a red, 5 pixel border around an HTML element, we could use this class:

<style>
  .thin-red-border {
    border-color: red;
    border-width: 10px;
    border-style: solid;
  }
</style>
Create a class called thick-green-border. This class should add a 10px, solid, green border around an HTML element. Apply the class to your cat photo.

Remember that you can apply multiple classes to an element using its class attribute, by separating each class name with a space. For example:

<img class="class1 class2">

# Basic CSS: Add Rounded Corners with border-radius
Your cat photo currently has sharp corners. We can round out those corners with a CSS property called border-radius.

You can specify a border-radius with pixels. Give your cat photo a border-radius of 10px.

Note: This challenge allows for multiple possible solutions. For example, you may add border-radius to either the .thick-green-border class or the .smaller-image class.

# Basic CSS: Make Circular Images with a border-radius
In addition to pixels, you can also specify the border-radius using a percentage.

Give your cat photo a border-radius of 50%.

# Basic CSS: Give a Background Color to a div Element
You can set an element's background color with the background-color property.

For example, if you wanted an element's background color to be green, you'd put this within your style element:

.green-background {
  background-color: green;
}
Create a class called silver-background with the background-color of silver. Assign this class to your div element.

# Basic CSS: Set the id of an Element
In addition to classes, each HTML element can also have an id attribute.

There are several benefits to using id attributes: You can use an id to style a single element and later you'll learn that you can use them to select and modify specific elements with JavaScript.

id attributes should be unique. Browsers won't enforce this, but it is a widely agreed upon best practice. So please don't give more than one element the same id attribute.

Here's an example of how you give your h2 element the id of cat-photo-app:

<h2 id="cat-photo-app">

Give your form element the id cat-photo-form.

# Basic CSS: Use an id Attribute to Style an Element

One cool thing about id attributes is that, like classes, you can style them using CSS.

However, an id is not reusable and should only be applied to one element. An id also has a higher specificity (importance) than a class so if both are applied to the same element and have conflicting styles, the styles of the id will be applied.

Here's an example of how you can take your element with the id attribute of cat-photo-element and give it the background color of green. In your style element:

#cat-photo-element {
  background-color: green;
}
Note that inside your `style` element, you always reference classes by putting a `.` in front of their names. You always reference ids by putting a `#` in front of their names.

Try giving your form, which now has the id attribute of cat-photo-form, a green background.

# Let's take a break from the cat photo app for a little while
    -work on stylingHtml branch

# Basic CSS: Adjust the Padding of an Element

Now let's put our Cat Photo App away for a little while and learn more about styling HTML.

You may have already noticed this, but all HTML elements are essentially little rectangles.

Three important properties control the space that surrounds each HTML element: padding, border, and margin.

An element's padding controls the amount of space between the element's content and its border.

Here, we can see that the blue box and the red box are nested within the yellow box. Note that the red box has more padding than the blue box.

When you increase the blue box's padding, it will increase the distance (padding) between the text and the border around it.

Change the padding of your blue box to match that of your red box.

# Basic CSS: Adjust the Margin of an Element

An element's margin controls the amount of space between an element's border and surrounding elements.

Here, we can see that the blue box and the red box are nested within the yellow box. Note that the red box has a bigger margin than the blue box, making it appear smaller.

When you increase the blue box's margin, it will increase the distance between its border and surrounding elements.

Change the margin of the blue box to match that of the red box.

# Basic CSS: Add a Negative Margin to an Element
An element's margin controls the amount of space between an element's border and surrounding elements.

If you set an element's margin to a negative value, the element will grow larger.

Try to set the margin to a negative value like the one for the red box.

Change the margin of the blue box to -15px, so it fills the entire horizontal width of the yellow box around it.

# Basic CSS: Add Different Padding to Each Side of an Element
Sometimes you will want to customize an element so that it has different amounts of padding on each of its sides.

CSS allows you to control the padding of all four individual sides of an element with the padding-top, padding-right, padding-bottom, and padding-left properties.

Give the blue box a padding of 40px on its top and left side, but only 20px on its bottom and right side.

# Basic CSS: Add Different Margins to Each Side of an Element
Sometimes you will want to customize an element so that it has a different margin on each of its sides.

CSS allows you to control the margin of all four individual sides of an element with the margin-top, margin-right, margin-bottom, and margin-left properties.

Give the blue box a margin of 40px on its top and left side, but only 20px on its bottom and right side.

# Basic CSS: Use Clockwise Notation to Specify the Padding of an Element
Instead of specifying an element's padding-top, padding-right, padding-bottom, and padding-left properties individually, you can specify them all in one line, like this:

padding: 10px 20px 10px 20px;

These four values work like a clock: top, right, bottom, left, and will produce the exact same result as using the side-specific padding instructions.

Use Clockwise Notation to give the ".blue-box" class a padding of 40px on its top and left side, but only 20px on its bottom and right side.

# Basic CSS: Use Clockwise Notation to Specify the Margin of an Element
Let's try this again, but with margin this time.

Instead of specifying an element's margin-top, margin-right, margin-bottom, and margin-left properties individually, you can specify them all in one line, like this:

margin: 10px 20px 10px 20px;

These four values work like a clock: top, right, bottom, left, and will produce the exact same result as using the side-specific margin instructions.

Use Clockwise Notation to give the element with the blue-box class a margin of 40px on its top and left side, but only 20px on its bottom and right side.

# Finished the padding/margin section of CSS
    -back to the CatPhotoApp!

# Basic CSS: Use Attribute Selectors to Style Elements
You have been adding id or class attributes to elements that you wish to specifically style. These are known as ID and class selectors. There are other CSS Selectors you can use to select custom groups of elements to style.

Let's bring out CatPhotoApp again to practice using CSS Selectors.

For this challenge, you will use the [attr=value] attribute selector to style the checkboxes in CatPhotoApp. This selector matches and styles elements with a specific attribute value. For example, the below code changes the margins of all elements with the attribute type and a corresponding value of radio:

[type='radio'] {
  margin: 20px 0px 20px 0px;
}
Using the type attribute selector, try to give the checkboxes in CatPhotoApp a top margin of 10px and a bottom margin of 15px.

# Basic CSS: Understand Absolute versus Relative Units
The last several challenges all set an element's margin or padding with pixels (px). Pixels are a type of length unit, which is what tells the browser how to size or space an item. In addition to px, CSS has a number of different length unit options that you can use.

The two main types of length units are absolute and relative. Absolute units tie to physical units of length. For example, in and mm refer to inches and millimeters, respectively. Absolute length units approximate the actual measurement on a screen, but there are some differences depending on a screen's resolution.

Relative units, such as em or rem, are relative to another length value. For example, em is based on the size of an element's font. If you use it to set the font-size property itself, it's relative to the parent's font-size.

Note: There are several relative unit options that are tied to the size of the viewport. They are covered in the Responsive Web Design Principles section.

Add a padding property to the element with class red-box and set it to 1.5em.

# Basic CSS: Understand Absolute versus Relative Units
The last several challenges all set an element's margin or padding with pixels `(px)`. `Pixels` are a type of length unit, which is what tells the browser how to size or space an item. In addition to px, CSS has a number of different length unit options that you can use.

The two main types of length units are `absolute` and `relative`. `Absolute units` tie to physical units of length. For example, `in` and `mm` refer to inches and millimeters, respectively. Absolute length units approximate the actual measurement on a screen, but there are some differences depending on a screen's resolution.

Relative units, such as `em` or `rem`, are relative to another length value. For example, `em` is based on the size of an element's font. If you use it to set the `font-size` property itself, it's relative to the parent's `font-size`.

Note: There are several relative unit options that are tied to the size of the viewport. They are covered in the Responsive Web Design Principles section.

Add a padding property to the element with class red-box and set it to 1.5em.

# Basic CSS: Style the HTML Body Element
Now let's start fresh and talk about CSS inheritance.

Every HTML page has a body element.

We can prove that the body element exists here by giving it a background-color of black.

We can do this by adding the following to our style element:

body {
  background-color: black;
}

# Basic CSS: Inherit Styles from the Body Element
Now we've proven that every HTML page has a body element, and that its body element can also be styled with CSS.

Remember, you can style your body element just like any other HTML element, and all your other elements will inherit your body element's styles.

First, create a h1 element with the text Hello World

Then, let's give all elements on your page the color of green by adding color: green; to your body element's style declaration.

Finally, give your body element the font-family of monospace by adding font-family: monospace; to your body element's style declaration.

# Basic CSS: Prioritize One Style Over Another
Sometimes your HTML elements will receive multiple styles that conflict with one another.

For example, your h1 element can't be both green and pink at the same time.

Let's see what happens when we create a class that makes text pink, then apply it to an element. Will our class override the body element's color: green; CSS property?

Create a CSS class called pink-text that gives an element the color pink.

Give your h1 element the class of pink-text.

# Basic CSS: Override Styles in Subsequent CSS
Our "pink-text" class overrode our body element's CSS declaration!

We just proved that our classes will override the body element's CSS. So the next logical question is, what can we do to override our pink-text class?

Create an additional CSS class called blue-text that gives an element the color blue. Make sure it's below your pink-text class declaration.

Apply the blue-text class to your h1 element in addition to your pink-text class, and let's see which one wins.

Applying multiple class attributes to a HTML element is done with a space between them like this:

class="class1 class2"

Note: It doesn't matter which order the classes are listed in the HTML element.

However, the order of the class declarations in the <style> section is what is important. The second declaration will always take precedence over the first. Because .blue-text is declared second, it overrides the attributes of .pink-text

# Basic CSS: Override Class Declarations by Styling ID Attributes
We just proved that browsers read CSS from top to bottom in order of their declaration. That means that, in the event of a conflict, the browser will use whichever CSS declaration came last. Notice that if we even had put blue-text before pink-text in our h1 element's classes, it would still look at the declaration order and not the order of their use!

But we're not done yet. There are other ways that you can override CSS. Do you remember id attributes?

Let's override your pink-text and blue-text classes, and make your h1 element orange, by giving the h1 element an id and then styling that id.

Give your h1 element the id attribute of orange-text. Remember, id styles look like this:

<h1 id="orange-text">

Leave the blue-text and pink-text classes on your h1 element.

Create a CSS declaration for your orange-text id in your style element. Here's an example of what this looks like:

#brown-text {
  color: brown;
}
Note: It doesn't matter whether you declare this CSS above or below pink-text class, since id attribute will always take precedence.

# Basic CSS: Override Class Declarations with Inline Styles
So we've proven that id declarations override class declarations, regardless of where they are declared in your style element CSS.

There are other ways that you can override CSS. Do you remember inline styles?

Use an inline style to try to make our h1 element white. Remember, in line styles look like this:

<h1 style="color: green;">

Leave the blue-text and pink-text classes on your h1 element.

# Basic CSS: Override All Other Styles by using Important
Yay! We just proved that inline styles will override all the CSS declarations in your style element.

But wait. There's one last way to override CSS. This is the most powerful method of all. But before we do it, let's talk about why you would ever want to override CSS.

In many situations, you will use CSS libraries. These may accidentally override your own CSS. So when you absolutely need to be sure that an element has specific CSS, you can use !important

Let's go all the way back to our pink-text class declaration. Remember that our pink-text class was overridden by subsequent class declarations, id declarations, and inline styles.

Let's add the keyword !important to your pink-text element's color declaration to make 100% sure that your h1 element will be pink.

An example of how to do this is:

color: red !important;

# Basic CSS: Use Hex Code for Specific Colors
Did you know there are other ways to represent colors in CSS? One of these ways is called hexadecimal code, or hex code for short.

We usually use decimals, or base 10 numbers, which use the symbols 0 to 9 for each digit. Hexadecimals (or hex) are base 16 numbers. This means it uses sixteen distinct symbols. Like decimals, the symbols 0-9 represent the values zero to nine. Then A,B,C,D,E,F represent the values ten to fifteen. Altogether, 0 to F can represent a digit in hexadecimal, giving us 16 total possible values. You can find more information about hexadecimal numbers here.

In CSS, we can use 6 hexadecimal digits to represent colors, two each for the red (R), green (G), and blue (B) components. For example, #000000 is black and is also the lowest possible value. You can find more information about the RGB color system here.

body {
  color: #000000;
}
Replace the word black in our body element's background-color with its hex code representation, #000000.