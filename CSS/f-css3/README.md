# Adding CSS3 Features to HTML Pages
---
## Purpose

We designed this beginner's tutorial with the purpose of helping developers who are new to the CSS language and want to add extra look and feel to their HTML web pages. This tutorial covers CSS3 and the additional features that it provides. The goal is to show you how to implement these features in examples, not to provide an in-depth explanation for how each feature works.

**Note:** For an in-depth look into some of the features offered in CSS3, please look to the CSS3 Lecture Notes in the Modules folder.

### Getting Started: Prerequisites

All you need to get started is Text Editor, a Browser of choice, and some prior HTML and CSS knowledge.

- **Visual Studio Code**: For this tutorial, we will use Microsoft Visual Studio Code in order to edit our HTML code. You may choose to use another text editor if you feel comfortable doing so.

- **Google Chrome**: For this tutorial, we will use Google Chrome in order to view our HTML pages. You may choose another browser if you prefer.
  
-  **HTML Fundamentals**: For this tutorial, you will want at least a fundamental understanding of how HTML tags and elements work.

-  **CSS Fundamentals**: For this tutorial, you will want at least a fundamental understanding of how CSS properties work and can be added to an HTML element.

## Step 1: Set Up an HTML file

Follow previous instruction for creating an HTML file. To do so in Visual Studio Code, click on: New -> New File. Make sure to end the file name with .html to add the html file extension. Example:

    hello.html

Once the file is created, add any basic HTML elements you wish in preparation for adding CSS to these HTML Elements. For extensive details on CSS syntax please look at the CSS Fundamentals Lecture Notes in the modules folder.


## Step 2: Use the New CSS3 Features

Using the new features in CSS3 works very similar to your typical CSS syntax. We will use this example to outline a couple of examples that may have syntax you are not immediately familar with.


### Importing your own Fonts

CSS3 allows you to add an at-rule to define your own custom fonts you wish to use. Here is an example:

```
    @font-face {
        font-family: myFont;
        font-style: normal;
        font-weight: 400;
        src: url(MarvelRegular-Dj83.ttf);
    }
```

### Adding CSS3 Transitions

In CSS3, you can add a property to an element called `transition` that will define another property to be modified for a given length of time. We must then provide an event on the element that will trigger the transition and what value the property will be set to. See the following example:

    .highlight {
        transition: background-color 3s;
    }

    .highlight:hover {
        background-color: yellow;
    }

### Adding Flex Containers

CSS3 made it very easy to give your containers a flexible and reactive feel. All you have to do is make a class and use the flex container's new properties. Here is an example:

```
.flex-container {
  display: flex;
  flex-wrap: wrap;
  background-color: blue;
}
```