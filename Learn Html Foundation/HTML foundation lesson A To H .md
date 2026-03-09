HTML Foundations Lesson A

Almost all elements on an HTML page are just pieces of content wrapped in opening and closing HTML tags.

Opening tags tell the browser this is the start of an HTML element. They are comprised of a keyword enclosed in angle brackets <>. For example, an opening paragraph tag looks like this: <p>.

Closing tags tell the browser where an element ends. They are almost the same as opening tags; the only difference is that they have a forward slash before the keyword. For example, a closing paragraph tag looks like this: </p>.


Q-1 What are HTML tags?
Ans- HTML tags tell the browser what content an element contains.

HTML Foundations Lesson B

You can think of elements as containers for content. The opening and closing tags tell the browser what content the element contains. The browser can then use that information to determine how it should interpret and format the content.

There are some HTML elements that do not have a closing tag. These elements often look like this: <br /> or <img/>, but some can also be used without the closing forward slash such as <br> or <img>. These are known as void elements or empty elements because they don’t wrap any content. You will encounter a few of these in later lessons, but for the most part, elements will have both opening and closing tags.

HTML has a vast list of predefined tags that you can use to create all kinds of different elements. It is important to use the correct tags for content. Using the correct tags can have a big impact on two aspects of your sites: how they are ranked in search engines; and how accessible they are to users who rely on assistive technologies, like screen readers, to use the internet.

Using the correct elements for content is called semantic HTML. You will explore this in much more depth later on in the curriculum.

Q-2 Why are void elements like <br/> or <img> essential in HTML?
Ans- They indicate empty elements and require no closing tag.


HTML Foundations Lesson C

To demonstrate an HTML boilerplate, you first need an HTML file to work with.

Create a new folder on your computer and name it html-boilerplate. Within that folder create a new file and name it index.html.

You’re probably already familiar with a lot of different types of files, for example doc, pdf, and image files.

To let the computer know you want to create an HTML file, you need to append the filename with the .html extension as you have done when creating the index.html file.

It is worth noting that you named your HTML file index. You should always name the HTML file that will contain the homepage of your websites index.html. This is because web servers will by default look for an index.html page when users land on your websites - and not having one will cause big problems.

The DOCTYPE
Every HTML page starts with a doctype declaration. The doctype’s purpose is to tell the browser what version of HTML it should use to render the document. The latest version of HTML is HTML5, and the doctype for that version is simply <!DOCTYPE html>.

The doctypes for older versions of HTML were a bit more complicated. For example, this is the doctype declaration for HTML4:

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
However, you probably won’t ever want to be using an older version of HTML, and so you’ll always use <!DOCTYPE html>.

Open the index.html file created earlier in your text editor and add <!DOCTYPE html> to the very first line.

Q-1 What is the purpose of the DOCTYPE declaration?
Ans- it tell the browser which version of html to use to render the document.


HTML Foundations Lesson D

After you declare the doctype, you need to provide an <html> element. This is what’s known as the root element of the document, meaning that every other element in the document will be a descendant of it.

This becomes more important later on when you learn about manipulating HTML with JavaScript. For now, just know that the html element should be included on every HTML document.

Back in the index.html file, let’s add the <html> element by typing out its opening and closing tags, like so:

<!DOCTYPE html>
<html lang="en">
</html>
What is the lang attribute?
lang specifies the language of the text content in that element. This attribute is primarily used for improving accessibility of the webpage. It allows assistive technologies, for example screen readers, to adapt according to the language and invoke correct pronunciation.

Q-1 What is the html element?
ans- it is the root element in the document and all other elements should descend from it.


HTML Foundations Lesson E


The <head> element is where you put important meta-information about your webpages, and stuff required for your webpages to render correctly in the browser. Inside the <head>, you should not use any element that displays content on the webpage.

The Charset Meta Element
You should always have the meta tag for the charset encoding of the webpage in the head element: <meta charset="utf-8">.

Setting the encoding is very important because it ensures that the webpage will display special symbols and characters from different languages correctly in the browser.

Title Element
Another element you should always include in the head of an HTML document is the title element:

<title>My First Webpage</title>
The title element is used to give webpages a human-readable title which is displayed in your webpage’s browser tab.

If you didn’t include a title element, the webpage’s title would default to its file name. In your case that would be index.html, which isn’t very meaningful for users; this would make it very difficult to find your webpage if the user has many browser tabs open.

There are many more elements that can go within the head of an HTML document. However, for now it’s only crucial to know about the two elements you have covered here. You will introduce more elements that go into the head throughout the rest of the curriculum.

Back in index.html file, let’s add a head element with a charset meta element and a title within it. The head element goes within the HTML element and should always be the first element under the opening <html> tag:

<!DOCTYPE html>

<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>My First Webpage</title>
  </head>
</html>

Q-1 What is the purpose of the head element?
Ans- The head element is used to display important information about your webpage and is used to render web pages correctly with meta elements.



HTML Foundations Lesson F

The final element needed to complete the HTML boilerplate is the <body> element. This is where all the content that will be displayed to users will go - the text, images, lists, links, and so on.

To complete the boilerplate, add a body element to the index.html file. The body element also goes within the html element and is always below the head element, like so:

Q-1 What is the purpose of the body element?
Ans- This is where all content will be displayed on the page such images, text, and links.


HTML Foundations Lesson G

HTML and CSS are two languages that work together to create everything that you see when you look at something on the internet. HTML is the raw data that a webpage is built out of. All the text, links, cards, lists, and buttons are created in HTML. CSS is what adds style to those plain elements. HTML puts information on a webpage, and CSS positions that information, gives it color, changes the font, and makes it look great!

Q-1 What are the primary responsibilities of HTML and CSS in creating a webpage?
Ans- HTML structures the content, while CSS styles the elements.\


HTML Foundations Lesson H

HTML and CSS are primarily concerned with presenting information. They are not used to program logic. JavaScript, which you will learn in the next section, is used to make webpages do things. There is quite a lot you can do with just HTML and CSS, and you will definitely need them both. Throughout our curriculum, the following lessons focus on giving you the tools you need to succeed once you reach JavaScript content.

Q-1 What is one way in which JavaScript is different than HTML and CSS?What is one way in which JavaScript is different than HTML and CSS?
Ans- JavaScript makes webpages take actions.