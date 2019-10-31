# Programming with Javascript

Javascript is a language that adds dynamic content to a webpage.  You can insert Javascript throughout your Html to interact with the user and create a more attractive web page.  Similar to previous lessons on Html and CSS, Javascript contains its own set of rules and syntax.  While Html is for the content of your page and CSS is for the look and feel, Javascript is responsible for the interactive elements on a webpage.

Javascript is a language designed to solve a procedural problem, convert raw user data, and many more applications.  The extent of Javascript is limited by the programmer's imagination (within reason!). 

### Code Modularity

Here is an example of how Javascript might appear in your webpage.  There are many ways to intersperse Javascript in your Html.  I believe the best approach to adding Javascript is to keep your code modular.  This practice includes keeping your Javascript in separate files, and referring to them in the ```<head>``` tags of your Html as such:
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

Since I have the script loaded in the ```<head>``` tag of this Html, I can refer to the specific function.  This keeps my Html uncluttered and easy to read.  The function "displayGameScore" exists in the file "gamescore.js" and includes this code.
```
function displayGameScore() {
    // get LAFC and Sounder score
    var sounderScore = document.getElementById("sounderscore").value;
    var lafcScore = document.getElementById("lafcscore").value;

    // validate score values
    if (validateScores(sounderScore, lafcScore)) {
        
        // write values to page
        sounderScoreText.innerHTML= sounderScore; 
        lafcScoreText.innerHTML= lafcScore;

        // test scores to see if user entered correct scores
        checkGameScore(sounderScore, lafcScore);
    }
}

function checkGameScore(score1, score2) {
    // checks user input against game score and prints results to page
    if (score1 == 3 && score2 == 1) {
        scoreGuess.innerHTML = "That's the correct score!  Sounders won!";
    } else if (score1 != 3 && score2 == 1) {
        if (score1 > 3) {
            scoreGuess.innerHTML = "That's correct for LAFC!  But the Sounders scored LESS goals.";
        } else if (score1 < 3) {
            scoreGuess.innerHTML = "That's correct for LAFC!  But the Sounders scored MORE goals.";
        }
    } else if (score1 == 3 && score2 != 1) {
        if (score2 > 1) {
            scoreGuess.innerHTML = "That's correct score for the Sounders!  But LAFC scored LESS goals.";
        } else if (score2 < 1) {
            scoreGuess.innerHTML = "That's correct score for the Sounders!  But LAFC scored MORE goals.";
        }
    } else {
        scoreGuess.innerHTML = "Both of your scores are wrong.";
    }
}

function validateScores(score1, score2) {
    if (isNaN(score1)) {
        alert("Sounder's score must be a number");
        return false;
    } else if (isNaN(score2)) {
        alert("LAFC's score must be a number");
        return false;
    } else {
        return true
    }
}
```


[Back to Home Page](index.md)