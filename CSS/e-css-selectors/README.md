# Adding CSS Through Various Selectors
---
## Purpose

We designed this beginner's tutorial with the purpose of helping developers who are new to the CSS language and want to add extra look and feel to their HTML web pages. This tutorial covers CSS Selectors, so that you can further distinguish which elements in your HTML page you want to apply some CSS to. 

**Note:** To learn about all of the different CSS Selectors please see the CSS Selectors Lecture Notes in the Modules folder. The purpose of this is to provide examples of utilizing these various CSS Selectors and provide actual code for some of them in action.

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


## Step 2: Use CSS Selectors to add CSS Properties

Once you have an HTML file set up that you want to add CSS to, you are ready to use CSS Selectors. Provided below are some examples of using CSS Selectors. Look to the AddedSelectors.html for a live example.

**Note:** CSS Selectors can be used for Internal or External CSS.

### Element Selector Example
***

Here is an example using the element tag to select the element and apply CSS to it:

    h1 {
        text-align: center;
    }

**Note:** These properties will apply to all elements of that type within your HTML page.

### Id Selector Example
***

Here is an example using the element's `id` attribute to select the element and apply CSS to it:

    #myId {
        text-align: center;
    }

### Class Selector Example
***

Here is an example of using the element's `class` attribute to select the element and apply CSS to it:

    .myClass {
        border: 1px solid black;
    }

### Universal Selector Example
***

Here is an example of using the Universal selector to apply CSS to all elements of an HTML page:

    * {
        font-family: Times New Roman;
    }

### Attribute Selector Example
***

There are several ways you can use attributes on an HTML element as a means for selecting it for CSS declarations. Look to the CSS Selectors Lecture Notes for several various ways to use the Attribute Selector. Two such examples are provide below.

Select any element with a given attribute:

    [id] {
        background-color: yellow;
    }

Select any element with a given attribute equal to a specified value:

    [type="button"] {
        padding: 15px;
        text-align: center;
    }


### Grouping Selectors Example
***

You can group multiple elements together to apply common properties with the Grouping Selector Here is an example:

    h1, h2 {
        color: blue;
    }


**Note:** Many other selectors exist for niche situations. To learn about more selectors, see our CSS Selectors Lecture Notes in the Modules folder.

