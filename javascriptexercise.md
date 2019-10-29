# Intro to Javascript

In this exercise I learned how the **javascript** can be used to create dynamic web pages.  Similar to how HTML and CSS files are kept separate, JS code files are typically located in its own document.  This creates three distinct layers with three distinct features.  HTML is responsible for the way the content is presented, CSS is responsible for the look and feel of the page, and JS code is responsible for interacting with the users of your website.  

### Dot Notation

In Javascript, *objects* call their *methods* to produce a result.  Some programmeres call this style dot notation because the object calling its function is separated by a ```.``` such as:
```
document.write("hello world");
```
In this example, ```document``` refers to the object.  In this case it is the web page *document*.  The ```document``` object is being called using its ```write``` method.  The ```write``` method executes its code with the *aruments* or *parameters* in its parenthesis ```()```.  If this piece of code were included in a script, it would output ```hello world``` somewhere on the web page.