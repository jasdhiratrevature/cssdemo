# Integrating Bootstrap into Your Code
---
## Purpose

We designed this beginner's tutorial with the purpose of helping developers who are new to the CSS language and want to add some extra look and feel to their HTML web pages. This tutorial covers Bootstrap, a CSS library, and how you can use it within your HTML pages. 

**Note:** This example is intended to show you how to use Bootstrap. It will not teach you everything there is to know about how Bootstrap works. To learn more about Bootstrap, please look to the Bootstrap Lecture Notes in the Modules folder and the official documentation.


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

## Step 2: Add the Bootstrap library to your code


There are 2 ways to add Bootstrap into your code.

1. Download Bootstrap 4 - You can download the bootstrap from [getbootstrap.com](https://getbootstrap.com/). Then, you just have to add the library files into your project.
2. Include Bootstrap  from a CDN - You can skip the download with [BootstrapCDN](https://www.bootstrapcdn.com/) by copying the links and paste it in the head section of the html code. As of 07/2020 here is the following tags you would want to add inside of your `<head>` tag:

```
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css" integrity="sha384-9aIt2nRpC12Uk9gS9baDl411NQApFmC26EwAOH8WgZl5MYYxFfc+NcPb1dKGj7Sk" crossorigin="anonymous">

<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/js/bootstrap.min.js" integrity="sha384-OgVRvuATP1z7JjHLkuOU7Xw704+h835Lr+6QL9UvYjZE3Ipu6Tp75j7Bh/kR0JKI" crossorigin="anonymous"></script>
```

**Note:** The `<script>` tag is for adding Bootstrap JS library. If you choose to add this library you will also want to include the following tags:

```
<script src="https://code.jquery.com/jquery-3.5.1.slim.min.js" integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj" crossorigin="anonymous"></script>
<script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js" integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo" crossorigin="anonymous"></script>
```

**Note:** If you are using a Front-end Framework like Angular there are simpler ways to add in Bootstrap via package managers that you may wish to use. One such example for Angular is to use the Node Package Manager with the following code:

    npm install Bootstrap

## Step 3: Using Bootstrap

Once you have added Bootstrap to your code you have effectively added in a ton of preset class names with preset properties. All you have to do to use them is know what classes exist and then simply add them to your HTML elements.

**Note:** For an extensive list of Bootstrap's classes, please look to the Bootstrap Lecture Notes in the Modules folder.

**Note:** Bootstrap created a grid system used throughout the Framework and usable by developer. For information on the topic and its usage, look into the Bootstrap Lecture Notes in the Modules folder and in the official documentation.

Below are some examples of using some of the various Bootstrap properties. Look to the bootstrapEx.html file for a live example.

### Adding a Bootstrap Container

Bootstrap uses a container to organize the elements within it. You should surround all of your elements that you want to apply Bootstrap to within a container. Here is a example of creating one:

```
<div class="container">
    Add Elements Here
</div>
```

### Bootstrap Tables

There are many options that you have available for Bootstrap tables. Look to the Bootstrap Lecture Notes for more options. Here are two such examples:

```
<div class="container">
 <table class="table table-dark">
    ...
 </table>
</div>
```

```
<div class="container">
 <table class="table table-bordered table-striped table-hover">
    ...
 </table>
</div>
```

**Note:** You can concatenate options for an element together within the class name. All properties from all options will apply.


### Bootstrap Navbar

Another commonly used Bootstrap feature is their pre-built Navbar. Provided below is an example of how to use one:

```
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <a class="navbar-brand" href="#">Navbar</a>
  <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
    <div class="navbar-nav">
      <a class="nav-item nav-link active" href="#">Home</a>
      <a class="nav-item nav-link" href="#">Features</a>
    </div>
  </div>
</nav>
```

**Note:** There are many other pre-built features added by Bootstrap. To see some additional features and options available please look to the Bootstrap Lecture Notes.

