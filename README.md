# 4-1-Front_End_Dev

# 4.1 - Front-End Development

###### ICS3U - Mr. Jamieson 🐠

- Some of the basic lesson information is on my website: [www.brash.ca/ics3uc/4/1](https://sites.google.com/ocsb.ca/ics3u-ash/units/unit-4-modular-and-lists/4-1)
- Make sure you have installed the [Live Preview Extension](vscode:extension/ms-vscode.live-server) in VSCode.
  - After installing the extension, you _might_ want to go to the settings for it and change the `Open Preview Target` to "External Browser"

<br>

---


### Graphical User Interface - GUI
A web page (HTML file) is just like an application window (think Photoshop, Files, Spotify, etc). It has content (text or pictures) and interactivity (buttons, sliders, boxes). In fact, many apps on your phone or computer are actually web-pages because it's so easy to make a nice-looking interface with HTML.

- The **front-end** is the screen the user sees. It is created by _defining_ or _declaring_ **what** should be on the page and **where**.
- The **back-end** is any code we write to make the program interactive. When the user interacts with the front-end, the back-end does the work to _react_.

A GUI (document / page / app screen) has two major sections:

1. **The HEAD**. This is an invisible section that tells the web-browser or operating system specific instructions like the size of the window, if the scroll bars should be visible, the icon or title of the window, the language to display, etc... The user does not see this section.
2. **The BODY**. This is the actual page content that the _user_ will see and interact with.

### HTML

Let's take a look at a blank (empty) HTML document:
```HTML
<!DOCTYPE html>

<html>

  <head>

  </head>

  <body>

  </body>
  
</html>
```

The items you see inside arrow-brackets are called **Tags**. They are like a declaration or definition of a section or _thing_ on the document. **Let's break it down:**
```HTML
<!DOCTYPE html>   This tells the interpreter or browser that it should expect HTML tags.
```
```HTML
<html>  This is an opening tag to say "We are starting the actual HTML now"
```
```HTML
<head>
        These are the start and stop (open and close) tags for the HEAD section of the page.
        Anything between these tags will live in the hidden section of the page.
</head>
```
```HTML
<body>
        These are the open and close tags for the BODY section of the page.
        All content for the user to see will go between these tags.
</body>
```
```HTML
</html> This is the closing tag to say "Our page is complete."
```

### index.html

All web-servers need a "first page" to show when you visit the site. For example, when you go to [www.brash.ca](https://www.brash.ca) you are shown the `index.html` file. It is named after the "index" at the back of a book which displays where everything is.

In this project you have a blank [index.html](index.html) file waiting to be edited and viewed.
- To preview your page in an actual browser, right-click the file and select `Show Preview` (right now it's blank)
- The edit the file, normal-click on it to see the code in VSCode

### Our First Edits

Right now the page is blank and the title on the browser tab is `127.0.0.1:3000/index.html`. **Let's fix that**.
1. Inside the `<body>` of your page (between the open and closing BODY tags), place some text like "Hello World!" or "Hi Mom! 🥰"
2. Inside the `<head>` of your page, let's put a more interesting title for the browser tab.
   - Use the `<title>  </title>` tag to place a title on the browser tab/window. Whatever you place between them will display on the top bar of the browser (in an actual browser, not the interval VSCode preview window)
   - For example:
      ```HTML
      <head>
        <title>4.1 - HTML!</title>
      </head>
      ```

    Hopefully every time the HTML file is saved in VSCode, the preview automatically updates the page. If not, just hit the refresh button in the preview.

### Some HTML Basics

- HTML is not a _programming_ language. It is a _markup_ or _design_ language.
- HTML ignores white space. Try putting multiple lines of text inside your `<body>` like this:
  ```HTML
  Hello World!

  I love chocolate.
  ```
  You should notice that the text is all on one line on the actual page.
- The `<br>` tag can be used for a "break-line". It tells the browser to put the next content one line below. It's synonymous with `\n` for `console.log()`
  - The `<br>` tag _does not have a closing tag_. It is an _instruction_.
- Some of the more basic tags are:
  |Tag|Purpose|
  |:---:|---|
  |`<title>`Content`</title>`|This will place the `content` in the tab or top bar of the browser application window. **This tag must be placed inside the `<head>` of the page**|
  |`<h1>`Content`</h1>`|This is a **heading** tag - do not confuse this with the `<title>` tag. Headings can have 6 different sizes where `<h1>` is the largest and `<h6>` is the smallest. Try them out!|
  |`<b>`Content`</b>`|This will **bold** the content|
  |`<strong>`Content`</strong>`|This will also **bold** the content but has a slightly different meaning. This means that the content is very important|
  |`<i>`Content`</i>`|This will _italicize_ the content|
  |`<em>`Content`</em>`|This will also _italicize_ the content but similar to the `<strong>` tag, it has a level of _importance_ to it, describing the content as quite important|
  |`<p>`Content`</p>`|This is the _paragraph_ tag and is useful to separate text into paragraphs. By default it will put an empty line between paragraphs of text|
  |`<div>`Content`</div>`|One of the most-used tags, this is a _divider_ or _section_ or _container_ of content for the page. As you become used to HTML and styling your page you will learn to use these to break-up your content for different looks or areas on the page |
  |`<button>`Text`</button>`|This will place a clickable grey button with the `Text` written on it. For now the button will do nothing but we'll learn to make it react using JavaScript|
  |`<br>`|Insert a _break-line_|
  |`<hr>`|Insert a horizontal line across the page|
  |`<img>`|The image tag is used to insert a picture (jpg, png, etc) on the page.<br>It requires many **options**.<br>For Example: `<img src="myfile.png" width="200px">`|

Play around with the tags on your page and insert fake content. Try the different headers, paragraphs, divs, break-lines, etc... Maybe even try inserting a picture, if you can (but don't worry, we'll have a lesson on that next class).

### 🤔 What about the JavaScript file `script.js`?

Right now it is _not connected to our front-end_. It is useless... As we dive deeper into making a GUI with HTML, we will learn how to link the front-end and back-end. More on that later.
🐠
<br><br>
