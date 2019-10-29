# Intro to Javascript

In this exercise I learned how the **javascript** can be used to create dynamic web pages.  Similar to how HTML and CSS files are kept separate, JS code files are typically located in its own document.  This creates three distinct layers with three distinct features.  HTML is responsible for the way the content is presented, CSS is responsible for the look and feel of the page, and JS code is responsible for interacting with the users of your website.  Javascript is included in an HTML document by use of ```<script>``` tags.

### Statements 
A statement is just another name for a line of code in Javascript.
```
var username = "Micah";
```
In this example I am declaring a variable ```var``` with the name of ```username``` and I am storing the value of ```"Micah"``` in that variable.  From this point on in your script, if you use the value of ```username```, it will contain the last stored value ```Micah```.

### Block Notation
Javascript uses the curly braces ```{}``` to enclose statements.
```
if (username == "Micah") {
    // do something
} else {
    // do something else
}
```
In this example, if the value of ```username``` was "Micah", then all the code within the ```{}``` curly braces would be executed.  If the value was other than "Micah", the block of code would be passed over, and the ```else``` statement(s) would execute.

### Dot Notation

In Javascript, *objects* call their *methods* to produce a result.  Some programmers call this style dot notation because the object calling its function is separated by a ```.``` such as:
```
document.write("hello world");
```
In this example, ```document``` refers to the object.  In this case it is the web page *document*.  The ```document``` object is being called using its ```write``` method.  The ```write``` method executes its code with the *arguments* or *parameters* in its parenthesis ```()```.  If this piece of code were included in a script, it would output ```hello world``` somewhere on the web page.

