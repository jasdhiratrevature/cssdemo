# Integrating CSS Into Your Web Page
---
## Purpose

We designed this beginner's tutorial with the purpose of helping developers who are new to the CSS language and want to add extra look and feel to their HTML web pages. This tutorial covers CSS fundamentals such as basic CSS statements and enough information to get you started.

### Getting Started: Prerequisites

All you need to get started is Text Editor, a Browser of choice, and some prior HTML knowledge.

- **Visual Studio Code**: For this tutorial, we will use Microsoft Visual Studio Code in order to edit our HTML code. You may choose to use another text editor if you feel comfortable doing so.

- **Google Chrome**: For this tutorial, we will use Google Chrome in order to view our HTML pages. You may choose another browser if you prefer.
  
-  **HTML**: For this tutorial, you will want at least a fundamental understanding of how HTML tags and elements work.

## Step 1: Set Up an HTML file

Follow previous instruction for creating an HTML file. To do so in Visual Studio Code, click on: New -> New File. Make sure to end the file name with .html to add the html file extension. Example:

    hello.html

Once the file is created, add any basic HTML elements you wish in preparation for adding CSS to these HTML Elements. For extensive details on CSS syntax please look at the CSS Fundamentals Lecture Notes in the modules folder.

## Step 2: Adding Inline CSS

CSS can be added to your HTML Elements in three ways: Inline, Internal, and External. To add CSS inline, we must use the `style` attribute within an HTML element. The follow code is an example of adding CSS code inline to an HTML element.

    <h1 style="color: blue">Blue Header</h1>

**Note:** The code inside of the string for the `style` attribute is in CSS syntax. This CSS code is the declaration for the element at hand. In this case, for the H1 element.

## Step 3: Adding Internal CSS

**Note:** You can use any of the three approaches to adding CSS to your code. However CSS uses a cascade algorithm to determine which CSS is applied to the final product. The order in which they are applied are as follows: External -> Internal -> Inline. This means that any CSS added in Internal will override the External CSS if there is a conflict and Inline will override any External or Internal CSS if there is a conflict.

You can add Internal CSS by adding a `<style>` tag inside of your `<head>` tag of your HTML page. The code inside the `<style>` tag is recognized as CSS and will apply to the appropriate elements within that page.

**Note:** Since we aren't adding CSS directly to an element, as we did in Inline CSS, we will have to select what HTML element we want to apply our CSS to. A **selector** is a way for us to indicate what element(s) we want to use the succeeding CSS code for.

Here is the full syntax for CSS when use internally:

    selector {
        property: value;
    }

Here is an example using the element name as the selector:

    h1 {
        background-color: red;
    }

**Note:** This styling will apply to all `h1` tags in that HTML page.

**Note:** Other types of CSS Selectors will be addressed in the next Example: CSS Selectors

## Step 4: Adding External CSS Code

The last way to add CSS to your HTML elements is through the use of External CSS. This is accomplished in two phases. First, we create a separate CSS file:

    sample.css

We will add any desired CSS into this file. Then we must reference this CSS inside of our HTML file. We do so by adding a `<link>` tag into the `<head>` tag of our HTML page.

    <link rel="stylesheet" type="text/css" href="sample.css">

At this point you have the tools needed to add your own CSS. You just need to find out what properties you want to set to what values. Look to the Lecture Notes on some additional properties. Or go to this web site to see more: [CSS References](https://www.w3schools.com/cssref/)