# Design web pages with CSS

In this exercise I created an external CSS file to accomodate my web site.  This style sheet contains all the properties and their values for elements of my web page that I wish to control.  By using a style sheet, I have centralized the *look and feel* of my content in a customizable fashion.  Moving forward my index.html file contains no design or style elements.  While it is possible to have CSS located in the ```<head>```, I opted to create an external file and have my index refer to that file location.  This allows me to create multiple pages with the same style, creating a consistent **brand** for my website.

If you want to link an external CSS, you need to declare the location of your CSS file:
```
<link href="styles.css" type="text/css" rel="stylesheet" />
```

Then in my CSS file, I can create as many styles as I please in this format:
```
h1, h2, h3 {
    font-family: Arial, Helvetica, sans-serif;
    color: #1D252D;
```

In this example all my h1, h2, and h3 headers will be the specified font and will be displayed in a dark blue color.  CSS and Html accept colors by name, hex code, or even RGB code.  In this example I used a hex code that was supplied from the offical Seattle Sounders marketing page to suit my needs.
