Links and Images Lesson A
To get some practice using links and images throughout this lesson you need an HTML project to work with.

Create a new directory named odin-links-and-images.

Within that directory, create a new file named index.html.

Fill in the usual HTML boilerplate.

Finally, add the following h1 to the body: <h1>Homepage</h1>

Anchor Elements
To create a link in HTML, you use the anchor element. An anchor element is defined by wrapping the text or another HTML element you want to be a link with an <a> tag.

Add the following to the body of the index.html page you created and open it in the browser:

<a>click me</a>
You may have noticed that clicking this link doesn’t do anything. This is because an anchor tag on its own won’t know where you want to link to. You have to tell it a destination to go to. You do this by using an HTML attribute.

An HTML attribute gives additional information to an HTML element and always goes in the element’s opening tag. An attribute is usually made up of two parts: a name, and a value; however, not all attributes require a value. In your case, you need to add an href (hyperlink reference) attribute to the opening anchor tag. The value of the href attribute is the destination you want your link to go to.

Add the following href attribute to the anchor element you created previously and try clicking it again, don’t forget to refresh the browser so the new changes can be applied.

<a href="https://www.theodinproject.com/about">click me</a>
By default, any text wrapped with an anchor tag without an href attribute will look like plain text. If the href attribute is present, the browser will give the text a blue color and underline it to signify it is a link.

It’s worth noting you can use anchor tags to link to any kind of resource on the internet, not just other HTML documents. You can link to videos, pdf files, images, and so on, but for the most part, you will be linking to other HTML documents.

Links and Images Lesson B
To get some practice using links and images throughout this lesson you need an HTML project to work with.

Create a new directory named odin-links-and-images.

Within that directory, create a new file named index.html.

Fill in the usual HTML boilerplate.

Finally, add the following h1 to the body: <h1>Homepage</h1>

Anchor Elements
To create a link in HTML, you use the anchor element. An anchor element is defined by wrapping the text or another HTML element you want to be a link with an <a> tag.

Add the following to the body of the index.html page you created and open it in the browser:

<a>click me</a>
You may have noticed that clicking this link doesn’t do anything. This is because an anchor tag on its own won’t know where you want to link to. You have to tell it a destination to go to. You do this by using an HTML attribute.

An HTML attribute gives additional information to an HTML element and always goes in the element’s opening tag. An attribute is usually made up of two parts: a name, and a value; however, not all attributes require a value. In your case, you need to add an href (hyperlink reference) attribute to the opening anchor tag. The value of the href attribute is the destination you want your link to go to.

Add the following href attribute to the anchor element you created previously and try clicking it again, don’t forget to refresh the browser so the new changes can be applied.

<a href="https://www.theodinproject.com/about">click me</a>
By default, any text wrapped with an anchor tag without an href attribute will look like plain text. If the href attribute is present, the browser will give the text a blue color and underline it to signify it is a link.

It’s worth noting you can use anchor tags to link to any kind of resource on the internet, not just other HTML documents. You can link to videos, pdf files, images, and so on, but for the most part, you will be linking to other HTML documents.


What is an attribute?

An HTML attribute gives additional information to an HTML element and always goes in the element’s opening tag.


Links and Images Lesson C

To get some practice using links and images throughout this lesson you need an HTML project to work with.

Create a new directory named odin-links-and-images.

Within that directory, create a new file named index.html.

Fill in the usual HTML boilerplate.

Finally, add the following h1 to the body: <h1>Homepage</h1>

Anchor Elements
To create a link in HTML, you use the anchor element. An anchor element is defined by wrapping the text or another HTML element you want to be a link with an <a> tag.

Add the following to the body of the index.html page you created and open it in the browser:

<a>click me</a>
You may have noticed that clicking this link doesn’t do anything. This is because an anchor tag on its own won’t know where you want to link to. You have to tell it a destination to go to. You do this by using an HTML attribute.

An HTML attribute gives additional information to an HTML element and always goes in the element’s opening tag. An attribute is usually made up of two parts: a name, and a value; however, not all attributes require a value. In your case, you need to add an href (hyperlink reference) attribute to the opening anchor tag. The value of the href attribute is the destination you want your link to go to.

Add the following href attribute to the anchor element you created previously and try clicking it again, don’t forget to refresh the browser so the new changes can be applied.

<a href="https://www.theodinproject.com/about">click me</a>
By default, any text wrapped with an anchor tag without an href attribute will look like plain text. If the href attribute is present, the browser will give the text a blue color and underline it to signify it is a link.

It’s worth noting you can use anchor tags to link to any kind of resource on the internet, not just other HTML documents. You can link to videos, pdf files, images, and so on, but for the most part, you will be linking to other HTML documents.


What attribute tells links where to go to?
href


Links and Images Lesson D
Generally, there are two kinds of links you will create:

Links to pages on other websites on the internet

Links to pages located on your own websites
Absolute Links
Links to pages on other websites on the internet are called absolute links. A typical absolute link will be made up of the following parts: protocol://domain/path. An absolute link will always contain the protocol and domain of the destination.

You’ve already seen an absolute link in action. The link you created to The Odin Project’s About page earlier was an absolute link as it contains the protocol and domain.

https://www.theodinproject.com/about

Relative Links
Links to other pages within your own website are called relative links. Relative links do not include the domain name, since it is another page on the same site, it assumes the domain name will be the same as the page you created the link on.

Relative links only include the file path to the other page, relative to the page you are creating the link on. This is quite abstract, let’s see this in action using an example.

Within the odin-links-and-images directory, create another HTML file named about.html and paste the following code into it:

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Odin Links and Images</title>
  </head>

  <body>
    <h1>About Page</h1>
  </body>
</html>
Back in the index page, add the following anchor element to create a link to the about page:

<body>
  <h1>Homepage</h1>
	<a href="https://www.theodinproject.com/about">click me</a>

	<a href="about.html">About</a>
</body>
Open the index.html file in a browser and click on the about link to make sure it is all wired together correctly. Clicking the link should go to the about page you just created.

This works because the index and about page are in the same directory. That means you can simply use its name (about.html) as the link’s href value.

But you will usually want to organize your website directories a little better. Normally you would only have the index.html at the root directory and all other HTML files in their own directory.

Create a directory named pages within the odin-links-and-images directory and move the about.html file into this new directory.

Refresh the index page in the browser and then click on the about link. It will now be broken. This is because the location of the about page file has changed.

To fix this, you just need to update the about link href value to include the pages/ directory since that is the new location of the about.html file relative to the index.html file.

<body>
  <h1>Homepage</h1>
  <a href="pages/about.html">About</a>
</body>
Refresh the index page in the browser and try clicking the about link again, it should now be back in working order.

In many cases, this will work just fine; however, you can still run into unexpected issues with this approach. Prepending ./ before the link will in most cases prevent such issues. By adding ./ you are specifying to your code that it should start looking for the file/directory relative to the current directory.

<body>
  <h1>Homepage</h1>
  <a href="./pages/about.html">About</a>
</body>

What is the difference between an absolute and a relative link?
An absolute link is a link to another website. A relative link is a link another page on the current website.

Links and Images Lesson E
Websites would be fairly boring if they could only display text. Luckily HTML provides a wide variety of elements for displaying all sorts of different media. The most widely used of these is the image element.

To display an image in HTML you use the <img> element. Unlike the other elements you have encountered, the <img> is a void element. Empty, void HTML elements do not need a closing tag.

Instead of wrapping content with an opening and closing tag, it embeds an image into the page using a src attribute which tells the browser where the image file is located. The src attribute works much like the href attribute for anchor tags. It can embed an image using both absolute and relative paths.

For example, using an absolute path you can display an image located on The

To use images that you have on your own websites, you can use a relative path.

Create a new directory named images within the odin-links-and-images project.

Next, download this image and move it into the images directory you just created.

Rename the image to dog.jpg.

Finally add the image to the index.html file:

<body>
  <h1>Homepage</h1>
	<a href="https://www.theodinproject.com/about">click me</a>

	<a href="pages/about.html">About</a>

	<img src="images/dog.jpg">
</body>
Save the index.html file and open it in a browser to view Charles in all his glory.

Parent Directories
What if you want to use the dog image in the about page? You would first have to go up one level out of the pages directory into its parent directory so you could then access the images directory.

To go to the parent directory you need to use two dots in the relative filepath like this: ../. Let’s see this in action, within the body of the about.html file, add the following image below the heading you added earlier:

<img src="../images/dog.jpg">
To break this down:

First, you are going to the parent directory of the pages directory which is odin-links-and-images.

Then, from the parent directory, you can go into the images directory.

Finally, you can access the dog.jpg file.

Using the metaphor we used earlier, using ../ in a filepath is kind of like stepping out from the room you are currently in to the main hallway so you can go to another room.

Alt attribute
Besides the src attribute, every image element should also have an alt (alternative text) attribute.

The alt attribute is used to describe an image. It will be used in place of the image if it cannot be loaded. It is also used with screen readers to describe what the image is to visually impaired users.

This is how the The Odin Project logo example you used earlier looks with an alt attribute included:

Links and Images Lesson F

Websites would be fairly boring if they could only display text. Luckily HTML provides a wide variety of elements for displaying all sorts of different media. The most widely used of these is the image element.

To display an image in HTML you use the <img> element. Unlike the other elements you have encountered, the <img> is a void element. Empty, void HTML elements do not need a closing tag.

Instead of wrapping content with an opening and closing tag, it embeds an image into the page using a src attribute which tells the browser where the image file is located. The src attribute works much like the href attribute for anchor tags. It can embed an image using both absolute and relative paths.

For example, using an absolute path you can display an image located on The Odin Project site:

To use images that you have on your own websites, you can use a relative path.

Create a new directory named images within the odin-links-and-images project.

Next, download this image and move it into the images directory you just created.

Rename the image to dog.jpg.

Finally add the image to the index.html file:

<body>
  <h1>Homepage</h1>
	<a href="https://www.theodinproject.com/about">click me</a>

	<a href="pages/about.html">About</a>

	<img src="images/dog.jpg">
</body>
Save the index.html file and open it in a browser to view Charles in all his glory.

Parent Directories
What if you want to use the dog image in the about page? You would first have to go up one level out of the pages directory into its parent directory so you could then access the images directory.

To go to the parent directory you need to use two dots in the relative filepath like this: ../. Let’s see this in action, within the body of the about.html file, add the following image below the heading you added earlier:

<img src="../images/dog.jpg">
To break this down:

First, you are going to the parent directory of the pages directory which is odin-links-and-images.

Then, from the parent directory, you can go into the images directory.

Finally, you can access the dog.jpg file.

Using the metaphor we used earlier, using ../ in a filepath is kind of like stepping out from the room you are currently in to the main hallway so you can go to another room.

Alt attribute
Besides the src attribute, every image element should also have an alt (alternative text) attribute.

The alt attribute is used to describe an image. It will be used in place of the image if it cannot be loaded. It is also used with screen readers to describe what the image is to visually impaired users.

This is how the The Odin Project logo example you used earlier looks with an alt attribute included:


Links and Images Lesson G

Websites would be fairly boring if they could only display text. Luckily HTML provides a wide variety of elements for displaying all sorts of different media. The most widely used of these is the image element.

To display an image in HTML you use the <img> element. Unlike the other elements you have encountered, the <img> is a void element. Empty, void HTML elements do not need a closing tag.

Instead of wrapping content with an opening and closing tag, it embeds an image into the page using a src attribute which tells the browser where the image file is located. The src attribute works much like the href attribute for anchor tags. It can embed an image using both absolute and relative paths.

For example, using an absolute path you can display an image located on The Odin Project site:

To use images that you have on your own websites, you can use a relative path.

Create a new directory named images within the odin-links-and-images project.

Next, download this image and move it into the images directory you just created.

Rename the image to dog.jpg.

Finally add the image to the index.html file:

<body>
  <h1>Homepage</h1>
	<a href="https://www.theodinproject.com/about">click me</a>

	<a href="pages/about.html">About</a>

	<img src="images/dog.jpg">
</body>
Save the index.html file and open it in a browser to view Charles in all his glory.

Parent Directories
What if you want to use the dog image in the about page? You would first have to go up one level out of the pages directory into its parent directory so you could then access the images directory.

To go to the parent directory you need to use two dots in the relative filepath like this: ../. Let’s see this in action, within the body of the about.html file, add the following image below the heading you added earlier:

<img src="../images/dog.jpg">
To break this down:

First, you are going to the parent directory of the pages directory which is odin-links-and-images.

Then, from the parent directory, you can go into the images directory.

Finally, you can access the dog.jpg file.

Using the metaphor we used earlier, using ../ in a filepath is kind of like stepping out from the room you are currently in to the main hallway so you can go to another room.

Alt attribute
Besides the src attribute, every image element should also have an alt (alternative text) attribute.

The alt attribute is used to describe an image. It will be used in place of the image if it cannot be loaded. It is also used with screen readers to describe what the image is to visually impaired users.

This is how the The Odin Project logo example you used earlier looks with an alt attribute included:

Links and Images Lesson H
Websites would be fairly boring if they could only display text. Luckily HTML provides a wide variety of elements for displaying all sorts of different media. The most widely used of these is the image element.

To display an image in HTML you use the <img> element. Unlike the other elements you have encountered, the <img> is a void element. Empty, void HTML elements do not need a closing tag.

Instead of wrapping content with an opening and closing tag, it embeds an image into the page using a src attribute which tells the browser where the image file is located. The src attribute works much like the href attribute for anchor tags. It can embed an image using both absolute and relative paths.

For example, using an absolute path you can display an image located on The Odin Project site:

To use images that you have on your own websites, you can use a relative path.

Create a new directory named images within the odin-links-and-images project.

Next, download this image and move it into the images directory you just created.

Rename the image to dog.jpg.

Finally add the image to the index.html file:

<body>
  <h1>Homepage</h1>
	<a href="https://www.theodinproject.com/about">click me</a>

	<a href="pages/about.html">About</a>

	<img src="images/dog.jpg">
</body>
Save the index.html file and open it in a browser to view Charles in all his glory.

Parent Directories
What if you want to use the dog image in the about page? You would first have to go up one level out of the pages directory into its parent directory so you could then access the images directory.

To go to the parent directory you need to use two dots in the relative filepath like this: ../. Let’s see this in action, within the body of the about.html file, add the following image below the heading you added earlier:

<img src="../images/dog.jpg">
To break this down:

First, you are going to the parent directory of the pages directory which is odin-links-and-images.

Then, from the parent directory, you can go into the images directory.

Finally, you can access the dog.jpg file.

Using the metaphor we used earlier, using ../ in a filepath is kind of like stepping out from the room you are currently in to the main hallway so you can go to another room.

Alt attribute
Besides the src attribute, every image element should also have an alt (alternative text) attribute.

The alt attribute is used to describe an image. It will be used in place of the image if it cannot be loaded. It is also used with screen readers to describe what the image is to visually impaired users.

This is how the The Odin Project logo example you used earlier looks with an alt attribute included: