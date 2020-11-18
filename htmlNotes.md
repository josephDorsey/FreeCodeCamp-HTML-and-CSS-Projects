# Introduction to Basic HTML & HTML5

*What is HTML?*

`HTML`, or `HyperText Markup Language`, is a markup language used to describe the structure of a web page. It uses a special syntax or notation to organize and give information about the page to the browser. Elements usually have opening and closing tags that surround and give meaning to content. For example, there are different tag options to place around text to show whether it is a heading, a paragraph, or a list.

For example:

<h1>Top level heading: Maybe a page title</h1>

<p>A paragraph of text. Some information we would like to communicate to the viewer. This can be as long or short as we would like.</p>

<ol>
  <li>Number one on the list</li>
  <li>Number two</li>
  <li>A third item</li>
</ol>

# Basic HTML and HTML5: Headline with the h2 Element

Over the next few lessons, we'll build an HTML5 cat photo web app piece-by-piece.

The `h2` element you will be adding in this step will add a level two heading to the web page.

This element tells the browser about the structure of your website. h1 elements are often used for main headings, while `h2` elements are generally used for subheadings. There are also `h3`, `h4`, `h5` and `h6` elements to indicate different levels of subheadings.

# Basic HTML and HTML5: Inform with the Paragraph Element

`p` elements are the preferred element for paragraph text on websites. `p` is short for "paragraph".

You can create a paragraph element like this:

<p>I'm a p tag!</p>


# Basic HTML and HTML5: Fill in the Blank with Placeholder Text
Web developers traditionally use lorem ipsum text as placeholder text. The lorem ipsum text is randomly scraped from a famous passage by Cicero of Ancient Rome.

Lorem ipsum text has been used as placeholder text by typesetters since the 16th century, and this tradition continues on the web.

Well, 5 centuries is long enough. Since we're building a CatPhotoApp, let's use something called "kitty ipsum text".

# Basic HTML and HTML5: Uncomment HTML
Commenting is a way that you can leave comments for other developers within your code without affecting the resulting output that is displayed to the end user.

Commenting is also a convenient way to make code inactive without having to delete it entirely.

Comments in HTML start with <!-- and end with a -->

# Basic HTML and HTML5: Comment out HTML
Remember that in order to start a comment, you need to use <!-- and to end a comment, you need to use -->

Here you'll need to end the comment before your h2 element begins.

Comment out your h1 element and your p element, but not your h2 element.

# Basic HTML and HTML5: Introduction to HTML5 Elements
HTML5 introduces more descriptive HTML tags. These include main, header, footer, nav, video, article, section and others.

These tags give a descriptive structure to your HTML, make your HTML easier to read, and help with Search Engine Optimization (SEO) and accessibility. The main HTML5 tag helps search engines and other developers find the main content of your page.

Example usage, a main element with two child elements nested inside it:

<main> 
  <h1>Hello World</h1>
  <p>Hello Paragraph</p>
</main>

Note: Many of the new HTML5 tags and their benefits are covered in the Applied Accessibility section.

Create a second p element after the existing p element with the following kitty ipsum text: Purr jump eat the grass rip the couch scratched sunbathe, shed everywhere rip the couch sleep in the sink fluffy fur catnip scratched.

Then, create a main element and nest the two p elements inside the main element.

# Basic HTML and HTML5: Add Images to Your Website
You can add images to your website by using the img element, and point to a specific image's URL using the src attribute.

An example of this would be:

<img src="https://www.freecatphotoapp.com/your-image.jpg">

Note that img elements are self-closing.

All img elements must have an alt attribute. The text inside an alt attribute is used for screen readers to improve accessibility and is displayed if the image fails to load.

Note: If the image is purely decorative, using an empty alt attribute is a best practice.

Ideally the alt attribute should not contain special characters unless needed.

Let's add an alt attribute to our img example above:

<img src="https://www.freecatphotoapp.com/your-image.jpg" alt="A business cat wearing a necktie.">

Let's try to add an image to our website:

Within the existing main element, insert an img element before the existing p elements.

Now set the src attribute so that it points to this url:

https://bit.ly/fcc-relaxing-cat

Finally, don't forget to give your img element an alt attribute with applicable text.