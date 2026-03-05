Working With Text Lesson A

What would you expect the following text to output on an HTML page?

Example Code
<body>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
  incididunt ut labore et dolore magna aliqua.

  Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
  nisi ut aliquip ex ea commodo consequat.
</body>
It looks like two paragraphs of text, and so you might expect it to display in that way. However that is not the case, as you can see in the output below:


When the browser encounters new lines like this in your HTML, it will compress them down into one single space. The result of this compression is that all of the text is clumped together into one long line.

If you want to create paragraphs in HTML, you need to use the paragraph element, which will add a newline after each of your paragraphs. A paragraph element is defined by wrapping text content with a <p> tag.

Changing our example from before to use paragraph elements fixes the issue:


Working With Text Lesson B

Headings are different from other HTML text elements: they are displayed larger and bolder than other text to signify that they are headings.

There are 6 different levels of headings starting from <h1> to <h6>. The number within a heading tag represents that heading’s level. The largest and most important heading is h1, while h6 is the tiniest heading at the lowest level.

Headings are defined much like paragraphs. For example, to create an h1 heading, we wrap our heading text in a <h1> tag.

<html>
  <head>
  </head>
  <body>
    <h1>This is a heading 1</h1>
    <h2>This is a heading 2</h2>
    <h3>This is a heading 3</h3>
    <h4>This is a heading 4</h4>
    <h5>This is a heading 5</h5>
    <h6>This is a heading 6</h6>
  </body>
 </html>

Using the correct level of heading is important as levels provide a hierarchy to the content. An h1 heading should always be used for the heading of the overall page, and the lower level headings should be used as the headings for content in smaller sections of the page.

Q-1 How many different levels of headings are there and what is the difference between them?
Ans- There are 6 different levels of headings. h1 is the largest and most important heading, and h6 is the smallest and least important heading.


Working With Text Lesson C


The <strong> element makes text bold. It also semantically marks text as important; this affects tools, like screen readers, that users with visual impairments will rely on to use your website. The tone of voice on some screen readers will change to communicate the importance of the text within a strong element. To define a strong element you wrap text content in a <strong> tag.

You can use strong on its own:
<html>
  <head>
  </head>
  <body>
    <strong>Lorem ipsum dolor</strong>
   </body>
 </html>

 But you will probably find yourself using the strong element much more in combination with other text elements, like this

 <html>
  <head>
  </head>
  <body>
    <p>Lorem ipsum <strong>dolor sit</strong> amet, consectetur adipiscing elit.</p>
  </body>
</html>

Sometimes you will want to make text bold without giving it an important meaning. You’ll learn how to do that in the CSS lessons later in the curriculum.


Working With Text Lesson D


The em element makes text italic. It also semantically places emphasis on the text, which again may affect things like screen readers. To define an emphasized element you wrap text content in an <em> tag.

To use em on its own:
<html>
  <head>
  </head>
  <body>
    <em>Some emphasized text</em>
  </body>
 </html>

 Again, like the strong element, you will find yourself mostly using the em element with other text elements:
 <html>
  <head>
  </head>
  <body>
    <p>Lorem ipsum <em>dolor sit</em> amet, consectetur adipiscing elit.</p>
  </body>
 </html>



Working With Text Lesson E

You may have noticed that in all the examples in this lesson you indent any elements that are within other elements. This is known as nesting elements.

When you nest elements within other elements, you create a parent and child relationship between them. The nested elements are the children and the element they are nested within is the parent.

In the following example, the body element is the parent and the p is the child:
<html>
  <head>
  </head>
  <body>
    <p>Lorem ipsum dolor sit amet.</p>
  </body>
 </html>

 Just as in human relationships, HTML parent elements can have many children. Elements at the same level of nesting are considered to be siblings.

For example, the two p elements in the following code are siblings, since they are both children of the body tag and are at the same level of nesting as each other:
<html>
  <head>
  </head>
  <body>
    <p>Lorem ipsum dolor sit amet.</p>
    <p>Ut enim ad minim veniam.</p>
  </body>
 </html>

 You use indentation to make the level of nesting clear and readable for yourselves and other developers who will work with your HTML in the future. It is recommended to indent any child elements by two spaces.

The parent, child, and sibling relationships between elements will become much more important later when you start styling your HTML with CSS and adding behavior with JavaScript. For now, however, it is just important to know the distinction between how elements are related and the terminology used to describe their relationships.

Q-1 What relationship do two elements have if they are at the same level of nesting?
Ans-The element are Sibiling.


Working With Text Lesson F

You may have noticed that in all the examples in this lesson you indent any elements that are within other elements. This is known as nesting elements.

When you nest elements within other elements, you create a parent and child relationship between them. The nested elements are the children and the element they are nested within is the parent.

In the following example, the body element is the parent and the paragraph is the child:
<html>
  <head>
  </head>
  <body>
    <p>Lorem ipsum dolor sit amet.</p>
  </body>
 </html>

 Just as in human relationships, HTML parent elements can have many children. Elements at the same level of nesting are considered to be siblings.

For example, the two paragraphs in the following code are siblings, since they are both children of the body tag and are at the same level of nesting as each other:
<html>
  <head>
  </head>
  <body>
    <p>Lorem ipsum dolor sit amet.</p>
    <p>Ut enim ad minim veniam.</p>
  </body>
 </html>

 You use indentation to make the level of nesting clear and readable for yourselves and other developers who will work with your HTML in the future. It is recommended to indent any child elements by two spaces.

The parent, child, and sibling relationships between elements will become much more important later when you start styling your HTML with CSS and adding behavior with JavaScript. For now, however, it is just important to know the distinction between how elements are related and the terminology used to describe their relationships.

Q-1 What relationship does an element have with any nested element within it?
Ans- The element within the other element is called the child element.


Working With Text Lesson G
HTML comments are not visible to the browser; they allow us to comment on your code so that other developers or your future selves can read them and get some context about something that might not be clear in the code.

Writing an HTML comment is simple: You just enclose the comment with <!-- and -->tags. For example:

Example Code
<h1> View the html to see the hidden comments </h1>

<!-- I am a html comment -->

<p>Some paragraph text</p>

<!-- I am another html comment -->

Working With Text Lesson H

If you want to have a list of items where the order doesn’t matter, like a shopping list of items that can be bought in any order, then you can use an unordered list.

Unordered lists are created using the <ul> element, and each item within the list is created using the list item element <li>.

Each list item in an unordered list begins with a bullet point:
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>

If you instead want to create a list of items where the order does matter, like step-by-step instructions for a recipe, or your top 10 favorite TV shows, then you can use an ordered list.

Ordered lists are created using the <ol> element. Each individual item in them is again created using the list item element <li>. However, each list item in an ordered list begins with a number instead:
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>

Assignments
Watch the first three minutes of Kevin Powell's video on Ordered and Unordered lists above.


Make an unordered shopping list of your favorite foods.


Make an ordered list of todo’s you need to get done today.


Make an unordered list of places you’d like to visit someday.


Make an ordered list of your all time top 5 favorite video games or movies.

Q-1 What HTML tag is used to create an unordered list?
Ans- Ul

Working With Text Lesson I


If you want to have a list of items where the order doesn’t matter, like a shopping list of items that can be bought in any order, then you can use an unordered list.

Unordered lists are created using the <ul> element, and each item within the list is created using the list item element <li>.

Each list item in an unordered list begins with a bullet point:
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>

If you instead want to create a list of items where the order does matter, like step-by-step instructions for a recipe, or your top 10 favorite TV shows, then you can use an ordered list.

Ordered lists are created using the <ol> element. Each individual item in them is again created using the list item element <li>. However, each list item in an ordered list begins with a number instead:
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>

Q-1 What HTML tag is used to create an ordered list?
Ans- Ol


Working With Text Lesson J


If you want to have a list of items where the order doesn’t matter, like a shopping list of items that can be bought in any order, then you can use an unordered list.

Unordered lists are created using the <ul> element, and each item within the list is created using the list item element <li>.

Each list item in an unordered list begins with a bullet point:
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>


If you instead want to create a list of items where the order does matter, like step-by-step instructions for a recipe, or your top 10 favorite TV shows, then you can use an ordered list.

Ordered lists are created using the <ol> element. Each individual item in them is again created using the list item element <li>. However, each list item in an ordered list begins with a number instead:
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>