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

# Basic HTML and HTML5: Link to External Pages with Anchor Elements
You can use a (anchor) elements to link to content outside of your web page.

a elements need a destination web address called an href attribute. They also need anchor text. Here's an example:

<a href="https://freecodecamp.org">this links to freecodecamp.org</a>

Then your browser will display the text "this links to freecodecamp.org" as a link you can click. And that link will take you to the web address https://www.freecodecamp.org.

Create an a element that links to https://freecatphotoapp.com and has "cat photos" as its anchor text.

# Basic HTML and HTML5: Link to Internal Sections of a Page with Anchor Elements
a (anchor) elements can also be used to create internal links to jump to different sections within a webpage.

To create an internal link, you assign a link's href attribute to a hash symbol # plus the value of the id attribute for the element that you want to internally link to, usually further down the page. You then need to add the same id attribute to the element you are linking to. An id is an attribute that uniquely describes an element.

Below is an example of an internal anchor link and its target element:

<a href="#contacts-header">Contacts</a>
...
<h2 id="contacts-header">Contacts</h2>
When users click the Contacts link, they'll be taken to the section of the webpage with the Contacts header element.

Change your external link to an internal link by changing the href attribute to "#footer" and the text from "cat photos" to "Jump to Bottom".

Remove the target="_blank" attribute from the anchor tag since this causes the linked document to open in a new window tab.

Then add an id attribute with a value of "footer" to the <footer> element at the bottom of the page.

# Basic HTML and HTML5: Nest an Anchor Element within a Paragraph
You can nest links within other text elements.

<p>
  Here's a <a target="_blank" href="http://freecodecamp.org"> link to freecodecamp.org</a> for you to follow.
</p>
Let's break down the example: Normal text is wrapped in the p element:
<p> Here's a ... for you to follow. </p> Next is the anchor element <a> (which requires a closing tag </a>):
<a> ... </a> target is an anchor tag attribute that specifies where to open the link and the value "_blank" specifies to open the link in a new tab href is an anchor tag attribute that contains the URL address of the link:
<a href="http://freecodecamp.org"> ... </a> The text, "link to freecodecamp.org", within the a element called anchor text, will display a link to click:
<a href=" ... ">link to freecodecamp.org</a> The final output of the example will look like this:

Here's a link to freecodecamp.org for you to follow.

Nest the existing a element within a new p element. The new paragraph should have text that says "View more cat photos", where "cat photos" is a link, and the rest is plain text.

# Basic HTML and HTML5: Make Dead Links Using the Hash Symbol

Sometimes you want to add a elements to your website before you know where they will link.

This is also handy when you're changing the behavior of a link using JavaScript, which we'll learn about later.

The current value of the href attribute is a link that points to "https://freecatphotoapp.com". Replace the href attribute value with a #, also known as a hash symbol, to create a dead link.

For example: href="#"

# Basic HTML and HTML5: Turn an Image into a Link
You can make elements into links by nesting them within an a element.

Nest your image within an a element. Here's an example:

<a href="#"><img src="https://bit.ly/fcc-running-cats" alt="Three kittens running towards the camera."></a>

Remember to use # as your a element's href property in order to turn it into a dead link.

Place the existing image element within an a (anchor) element.

Once you've done this, hover over your image with your cursor. Your cursor's normal pointer should become the link clicking pointer. The photo is now a link.

# Basic HTML and HTML5: Create a Bulleted Unordered List
HTML has a special element for creating unordered lists, or bullet point style lists.

Unordered lists start with an opening <ul> element, followed by any number of <li> elements. Finally, unordered lists close with a </ul>

For example:

<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>
would create a bullet point style list of "milk" and "cheese".

Remove the last two p elements and create an unordered list of three things that cats love at the bottom of the page.

# Basic HTML and HTML5: Create an Ordered List
HTML has another special element for creating ordered lists, or numbered lists.

Ordered lists start with an opening <ol> element, followed by any number of <li> elements. Finally, ordered lists are closed with the </ol> tag.

For example:

<ol>
  <li>Garfield</li>
  <li>Sylvester</li>
</ol>
would create a numbered list of "Garfield" and "Sylvester".

Create an ordered list of the top 3 things cats hate the most.

# Basic HTML and HTML5: Create a Text Field
Now let's create a web form.

input elements are a convenient way to get input from your user.

You can create a text input like this:

<input type="text">

Note that input elements are self-closing.

Create an input element of type text below your lists.

# Basic HTML and HTML5: Add Placeholder Text to a Text Field
Placeholder text is what is displayed in your input element before your user has inputted anything.

You can create placeholder text like so:

<input type="text" placeholder="this is placeholder text">

Note: Remember that input elements are self-closing.

Set the placeholder value of your text input to "cat photo URL".

# Basic HTML and HTML5: Create a Form Element
You can build web forms that actually submit data to a server using nothing more than pure HTML. You can do this by specifying an action on your form element.

For example:

<form action="/url-where-you-want-to-submit-form-data"></form>

Nest the existing input element inside a form element and assign "https://freecatphotoapp.com/submit-cat-photo" to the action attribute of the form element.

# Basic HTML and HTML5: Add a Submit Button to a Form
Let's add a submit button to your form. Clicking this button will send the data from your form to the URL you specified with your form's action attribute.

Here's an example submit button:

<button type="submit">this button submits the form</button>

Add a button as the last element of your form element with a type of submit, and "Submit" as its text.



# Basic HTML and HTML5: Use HTML5 to Require a Field
You can require specific form fields so that your user will not be able to submit your form until he or she has filled them out.

For example, if you wanted to make a text input field required, you can just add the attribute required within your input element, like this: <input type="text" required>

Make your text input a required field, so that your user can't submit the form without completing this field.

Then try to submit the form without inputting any text. See how your HTML5 form notifies you that the field is required?

# Basic HTML and HTML5: Create a Set of Radio Buttons
You can use radio buttons for questions where you want the user to only give you one answer out of multiple options.

Radio buttons are a type of input.

Each of your radio buttons can be nested within its own label element. By wrapping an input element inside of a label element it will automatically associate the radio button input with the label element surrounding it.

All related radio buttons should have the same name attribute to create a radio button group. By creating a radio group, selecting any single radio button will automatically deselect the other buttons within the same group ensuring only one answer is provided by the user.

Here's an example of a radio button:

<label> 
  <input type="radio" name="indoor-outdoor">Indoor 
</label>
It is considered best practice to set a for attribute on the label element, with a value that matches the value of the id attribute of the input element. This allows assistive technologies to create a linked relationship between the label and the child input element. For example:

<label for="indoor"> 
  <input id="indoor" type="radio" name="indoor-outdoor">Indoor 
</label>
Add a pair of radio buttons to your form, each nested in its own label element. One should have the option of indoor and the other should have the option of outdoor. Both should share the name attribute of indoor-outdoor to create a radio group.

# Basic HTML and HTML5: Create a Set of Checkboxes
Forms commonly use checkboxes for questions that may have more than one answer.

Checkboxes are a type of input.

Each of your checkboxes can be nested within its own label element. By wrapping an input element inside of a label element it will automatically associate the checkbox input with the label element surrounding it.

All related checkbox inputs should have the same name attribute.

It is considered best practice to explicitly define the relationship between a checkbox input and its corresponding label by setting the for attribute on the label element to match the id attribute of the associated input element.

Here's an example of a checkbox:

<label for="loving"><input id="loving" type="checkbox" name="personality"> Loving</label>

Add to your form a set of three checkboxes. Each checkbox should be nested within its own label element. All three should share the name attribute of personality.



