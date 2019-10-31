# Programming with Javascript

Javascript is a language that adds dynamic content to a webpage.  You can insert Javascript throughout your Html to interact with the user and create a more attractive web page.  Similar to previous lessons on Html and CSS, Javascript contains its own set of rules and syntax.  While Html is for the content of your page and CSS is for the look and feel, Javascript is responsible for the interactive elements on a webpage.

Javascript is a language designed to solve a procedural problem, convert raw user data, and many more applications.  The extent of Javascript is limited by the programmer's imagination (within reason!). 

### Code Modularity

Here is an example of how Javascript might appear in your webpage.  There are many ways to intersperse Javascript in your Html.  I believe the best approach to adding Javascript is to keep your code modular.  This practice includes keeping your Javascript in seperate files, and refering to them in the ```<head>``` tags of your Html as such:
```
<head>
.... // other 
..  // stuff
<script src="js/gamescore.js"></script>
```
With the relative path to my script specified, I can now use the functions within that file in my Html.  In this example I have a button that *calls* the function in my script.
```
<input type="submit" value="Submit Scores" onclick="displayGameScore();">
```

Since I have the script loaded in the ```<head>``` tag of this Html, I can refer to the specific function.  This keeps my Html uncluttered and easy to read.


[Back to Home Page](index.md)