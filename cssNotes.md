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

