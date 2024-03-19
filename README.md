# Cat Facts API Example
In this brief tutorial, you will use a public API to display a random cat
fact on a web page.

## Exploring the API
Use a web browser to explore the Cat Fact API at https://catfact.ninja

1. Open Firefox or another a web browser.
2. Paste https://catfact.ninja into the address bar.
3. Explore the documentation for `/fact`
4. Paste https://catfact.ninja/fact into the address bar.
5. Observe the output returned. Pay particular attention to the _fact:_
   attribute.

The output from https://catfact.ninja/fact is in a format called JSON,
which is an acronym for (JavaScript Object Notation.) JavaScript is the
programming language used by web browsers, so it's relatively easy to
display a JSON-based cat fact in a web page.

## Building the Web Page
The cat fact web page will be built in stages. This is called an
_iterative development process_ and will let us check our progress
along the way, rather than just hoping everything works out.

### Step 1: The Web Page Template
This tutorial is about using an API to display information. So while
understanding HTML is useful, it's not the primary focus. To that end,
we'll simply download a predefined template and modify it.

You can find the template at:

https://github.com/DavesCodeMusings/cat-fact/blob/main/step1.html

Download the file and open it in Firefox or another web browser. You
should see a message like the following:

```
This is just a template. It doesn't do anything yet.
```

Now open the file in Visual Studio Code or another editor. You'll be
able to see the HTML used to display that simple message.

### Step 2: Calling the API
When calling an API directly from a web page using JavaScript, we'll
use a built-in function called `fetch`. You can find out more about
fetch from the official documentation maintained by Mozilla.

https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch

In much the same way we borrowed our HTML code from a template, we'll
borrow our JavaScript code from the Mozilla example. Their example is
about movies. Ours is about cats. We just need to do a little editing.

If you're a JavaScript pro, you can try this on your own. For the rest
of us, take a look at the step 2 example provided.

https://github.com/DavesCodeMusings/cat-fact/blob/main/step2.html

Download the file (or modify step1.html) and open it up in your web
browser. You should see something like the following message:

```
Open the browser's developer tools (CTRL + SHIFT + I) to view the console output.
```

Go ahead and open the developer tools and select the Console tab.
You should see a random cat fact displayed.

### Step 3: Displaying the API Response
Nobody wants to go to a web page that tells them to open developer tools
to see the information they came for. In this step, we'll take the API
response and show it on the page.

We've already got an HTML paragraph element displaying a message in the
file we downloaded. All we have to do is modify it to update dynamically
with the cat fact.

The trick is to assign an _id_ to the paragraph and then use JavaScript's
`document.getElementById()` function along with the innerHTML property
to change the text. Or you can just download step 3.

https://github.com/DavesCodeMusings/cat-fact/blob/main/step3.html

### Step 4: Making it Look Nice
You now get a random cat fact when you load the page into a browser.
But, it's just plain text and not very nice looking. In this step, we'll
add some Cascading Style Sheet CSS) code to dress it up. This isn't
required for the API to function, it's just a nice way to finish up.

The key elements here are a nice cat picture background from
Wikimedia Commons and a little formatting of the text style. If you're
familiar with CSS, you can make the changes on your own. Otherwise,
feel free to download the step 4 file.

https://github.com/DavesCodeMusings/cat-fact/blob/main/step4.html

## The Finished Product
See the final version of the cat fact web page here:

https://davescodemusings.github.io/cat-fact/

## Next Steps
Search the internet for the phrase "public api for testing" and browse
through some of the sites returned. Find an API that provides information
you find interesting. Modify the project created in this tutorial to
display the information gathered from your chosen API.
