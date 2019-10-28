# Html Exercise

[Hey, I'm not the most design-oriented programmer out there, but check out my site anyways!](https://micahthor.github.io/code102HTMLex/)


In this exercise I built a small website featuring my favorite soccer team, the Seattle Sounders.  Almost fifteen years ago I took a basic intro to web design course which helped in this assignment, but  HTML5 has come a long way from humble beginnings.  I think the most challenging part of creating a webpage is getting your content aligned.  Using a variety of styles becomes cumbersome if you don't keep your content in-check.  The process of this exercise involved a lot of trial and error, which translates to valuable learning experiences.  Overall I triumphed and was able to utilize many differebt html elements to create a *somewhat* visually striking webpage.  Enjoy!

One aspect of web design that I focused on for this project was to keep my style and content separated.  By using  ```<style>...</style>``` elements in the ```head``` section, I was able to focus all my content in the various elements of page's body.  I hope in future exercises to create a separate CSS file to further segregate the visual sources content from the content itself.

Here's what my style markup looked like for this project:
```
<style>
                header {
                    background-color: palegreen;
                    }
                nav {
                    text-align:center;
                    }
                nav ul {
                    display:inline-block;
                    }
                nav ul li {
                    display:inline-block;
                    margin-right: 20px;
                    }
                a {
                    font-family: Arial, Helvetica, sans-serif;
                }
                p, h1, h2, h3 {
                    font-family: Arial, Helvetica, sans-serif;
                }
                img {
                    display: block;
                    margin: 0 auto;
                }
                aside {
                    float: right;
                    padding: 0px 100px 0px 10px;
                    }
                footer {
                    text-align: center;
                }
        </style>
```

[Back to Home Page](index.md)