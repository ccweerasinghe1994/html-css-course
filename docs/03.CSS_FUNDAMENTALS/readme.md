### Introduction to CSS

![](../images/11.png)
![](../images/12.png)

### Inline, Internal and External CSS

#### inline css

this is not a good practice to use inline css

```html
<h2 style="color: blue">The Basic Language of the Web: HTML</h2>
```

#### internal css

if the styles become too long, this can be a bad practice

```html
<head>
  <meta charset="UTF-8" />
  <title>The Basic Language of the Web: HTML</title>
  <style>
    h1 {
      color: red;
    }
  </style>
</head>
```

#### external css

let's create a css file and link it to the html file

styles.css

```css
h1 {
  color: blue;
}
```

link that css file to the html file

```html
<head>
  <meta charset="UTF-8" />
  <title>The Basic Language of the Web: HTML</title>
  <link rel="stylesheet" href="styles.css" />
</head>
```

### Styling Text

let's style these text

```css
h1 {
  font-size: 26px;
  font-family: sans-serif;
  text-transform: uppercase;
  font-style: italic;
}

h2 {
  font-size: 40px;
  font-family: sans-serif;
}

h3 {
  font-size: 30px;
  font-family: sans-serif;
}

h4 {
  font-size: 20px;
  font-family: sans-serif;
  text-transform: uppercase;
  text-align: center;
}

p {
  font-size: 22px;
  font-family: sans-serif;
  line-height: 1.5;
}

li {
  font-family: sans-serif;
  font-size: 20px;
}
```

#### output

![](../images/13.png)

### Combining Selectors

```css
h1,
h2,
h3,
h4,
p,
li {
  font-family: sans-serif;
}
h1 {
  font-size: 26px;
  text-transform: uppercase;
  font-style: italic;
}

h2 {
  font-size: 40px;
}

h3 {
  font-size: 30px;
}

h4 {
  font-size: 20px;
  text-transform: uppercase;
  text-align: center;
}

p {
  font-size: 22px;
  line-height: 1.5;
}

li {
  font-size: 20px;
}
/* nested selectors */
footer p {
  font-size: 16px;
}

/* here we are encoding our html structure in to our css */
article header p {
  font-style: italic;
}
```

### Class and ID Selectors

let's add some classes and ids

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>The Basic Language of the Web: HTML</title>
    <link rel="stylesheet" href="styles.css" />
  </head>

  <body>
    <!--
    <h1>The Basic Language of the Web: HTML</h1>
    <h2>The Basic Language of the Web: HTML</h2>
    <h3>The Basic Language of the Web: HTML</h3>
    <h4>The Basic Language of the Web: HTML</h4>
    <h5>The Basic Language of the Web: HTML</h5>
    <h6>The Basic Language of the Web: HTML</h6>
    -->

    <header>
      <h1>📘 The Code Magazine</h1>

      <nav>
        <a href="blog.html">Blog</a>
        <a href="#">Challenges</a>
        <a href="#">Flexbox</a>
        <a href="#">CSS Grid</a>
      </nav>
    </header>

    <article>
      <header>
        <h2>The Basic Language of the Web: HTML</h2>

        <img
          src="img/laura-jones.jpg"
          alt="Headshot of Laura Jones"
          height="50"
          width="50"
        />

        <p id="author">
          Posted by <strong>Laura Jones</strong> on Monday, June 21st 2027
        </p>

        <img
          src="img/post-img.jpg"
          alt="HTML code on a screen"
          width="500"
          height="200"
        />
      </header>

      <p>
        All modern websites and web applications are built using three
        <em>fundamental</em>
        technologies: HTML, CSS and JavaScript. These are the languages of the
        web.
      </p>

      <p>
        In this post, let's focus on HTML. We will learn what HTML is all about,
        and why you too should learn it.
      </p>

      <h3>What is HTML?</h3>
      <p>
        HTML stands for <strong>H</strong>yper<strong>T</strong>ext
        <strong>M</strong>arkup <strong>L</strong>anguage. It's a markup
        language that web developers use to structure and describe the content
        of a webpage (not a programming language).
      </p>
      <p>
        HTML consists of elements that describe different types of content:
        paragraphs, links, headings, images, video, etc. Web browsers understand
        HTML and render HTML code as websites.
      </p>
      <p>In HTML, each element is made up of 3 parts:</p>

      <ol>
        <li>The opening tag</li>
        <li>The closing tag</li>
        <li>The actual element</li>
      </ol>

      <p>
        You can learn more at
        <a
          href="https://developer.mozilla.org/en-US/docs/Web/HTML"
          target="_blank"
          >MDN Web Docs</a
        >.
      </p>

      <h3>Why should you learn HTML?</h3>

      <p>
        There are countless reasons for learning the fundamental language of the
        web. Here are 5 of them:
      </p>

      <ul>
        <li>To be able to use the fundamental web dev language</li>
        <li>
          To hand-craft beautiful websites instead of relying on tools like
          Worpress or Wix
        </li>
        <li>To build web applications</li>
        <li>To impress friends</li>
        <li>To have fun 😃</li>
      </ul>

      <p>Hopefully you learned something new here. See you next time!</p>
    </article>

    <aside>
      <h4>Related posts</h4>

      <ul class="related">
        <li>
          <img
            src="img/related-1.jpg"
            alt="Person programming"
            width="75"
            width="75"
          />
          <a href="#">How to Learn Web Development</a>
          <p class="related-author">By Jonas Schmedtmann</p>
        </li>
        <li>
          <img src="img/related-2.jpg" alt="Lightning" width="75" heigth="75" />
          <a href="#">The Unknown Powers of CSS</a>
          <p class="related-author">By Jim Dillon</p>
        </li>
        <li>
          <img
            src="img/related-3.jpg"
            alt="JavaScript code on a screen"
            width="75"
            height="75"
          />
          <a href="#">Why JavaScript is Awesome</a>
          <p class="related-author">By Matilda</p>
        </li>
      </ul>
    </aside>

    <footer>
      <p id="copyright">Copyright &copy; 2027 by The Code Magazine.</p>
    </footer>
  </body>
</html>
```

let's style those classes and ids

```css
h1,
h2,
h3,
h4,
p,
li {
  font-family: sans-serif;
}
h1 {
  font-size: 26px;
  text-transform: uppercase;
  font-style: italic;
}

h2 {
  font-size: 40px;
}

h3 {
  font-size: 30px;
}

h4 {
  font-size: 20px;
  text-transform: uppercase;
  text-align: center;
}

p {
  font-size: 22px;
  line-height: 1.5;
}

li {
  font-size: 20px;
}
/* nested selectors */
/* footer p {
  font-size: 16px;
} */

#copyright {
  font-size: 16px;
  text-align: center;
}

/* here we are encoding our html structure in to our css */
article header p {
  font-style: italic;
  font-size: 18px;
}
/* here is a solution to the above problem */
#author {
  font-style: italic;
  font-size: 18px;
}

.related-author {
  font-size: 18px;
  font-weight: bold;
}

.related {
  list-style: none;
}
```

it's always better to use classes because then we are ready for the future.

### Working With Colors

![](../images/14.png)
![](../images/15.png)
![](../images/16.png)

```css
h1,
h2,
h3,
h4,
p,
li {
  font-family: sans-serif;
  color: #444;
}

h1,
h2,
h3 {
  color: #1098ad;
}

h1 {
  font-size: 26px;
  text-transform: uppercase;
  font-style: italic;
}

h2 {
  font-size: 40px;
}

h3 {
  font-size: 30px;
}

h4 {
  font-size: 20px;
  text-transform: uppercase;
  text-align: center;
}

p {
  font-size: 22px;
  line-height: 1.5;
}

li {
  font-size: 20px;
}
/* nested selectors */
/* footer p {
  font-size: 16px;
} */

#copyright {
  font-size: 16px;
  text-align: center;
}

/* here we are encoding our html structure in to our css */
article header p {
  font-style: italic;
  font-size: 18px;
}
/* here is a solution to the above problem */
#author {
  font-style: italic;
  font-size: 18px;
}

.related-author {
  font-size: 18px;
  font-weight: bold;
}

.related {
  list-style: none;
}

.main-header {
  background-color: #f7f7f7;
}

aside {
  background-color: #f7f7f7;
  border-top: 5px solid #1098ad;
  border-bottom: 5px solid #1098ad;
}
```

### Pseudo-classes

```css
li:first-child {
  font-weight: bold;
}

li:last-child {
  font-style: italic;
}

li:nth-child(even) {
  color: rebeccapurple;
}

article p:last-child {
  color: red;
}
```

### Styling Hyperlinks

### Using Chrome DevTools

### CSS Theory #1\_ Conflicts Between Selectors ### CSS Theory #2\_ Inheritance

and the Universal Selector ### CHALLENGE #1 ### CSS Theory #3\_ The CSS Box
Model ### Using Margins and Paddings ### Adding Dimensions ### Centering our
Page ### CHALLENGE #2 ### CSS Theory #4\_ Types of Boxes ### CSS Theory #5\_
Absolute Positioning ### Pseudo-elements ### Developer Skill #1\_ Googling and
Reading Documentation ### Developer Skill #2\_ Debugging and Asking Questions

### CHALLENGE #3

```

```

```

```
