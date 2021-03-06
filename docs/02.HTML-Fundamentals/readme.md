- [Introduction to HTML](#introduction-to-html)
- [HTML Document Structure](#html-document-structure)
- [Text Elements](#text-elements)
- [More Text Elements\_ Lists](#more-text-elements_-lists)
- [Images and Attributes](#images-and-attributes)
- [Hyperlinks](#hyperlinks)
- [Structuring our Page](#structuring-our-page)
- [A Note on Semantic HTML](#a-note-on-semantic-html)
- [CHALLENGE #1](#challenge-1)
- [CHALLENGE #2](#challenge-2)

### Introduction to HTML

![](../images/6.png)
![](../images/7.png)

### HTML Document Structure

basic html structure

```html
<!DOCTYPE html>
<html>
  <head>
    <title>basic language of the web:HTML</title>
  </head>
  <body>
    <h1>basic language of the web:HTML</h1>
  </body>
</html>
```

### Text Elements

h1 - h6

```html
<h1>This is a heading</h1>
<h2>This is a heading</h2>
<h3>This is a heading</h3>
<h4>This is a heading</h4>
<h5>This is a heading</h5>
<h6>This is a heading</h6>
```

adding first programme structure

```html
<!DOCTYPE html>
<html>
  <head>
    <title>basic language of the web:HTML</title>
  </head>
  <body>
    <h1>📘 The Code Magazine</h1>
    <p>Posted by <strong>Laura Jones</strong> on Monday, June 21st 2027</p>

    <h2>The Basic Language of the Web: HTML</h2>
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
      HTML stands for <strong>H</strong>yperText <strong>M</strong>arkup
      <strong>L</strong>anguage. It's a markup language that web developers use
      to structure and describe the content of a webpage (not a programming
      language).
    </p>
    <p>
      HTML consists of elements that describe different types of content:
      paragraphs, links, headings, images, video, etc. Web browsers understand
      HTML and render HTML code as websites.
    </p>
    <h3>Why should you learn HTML?</h3>
    <p></p>
  </body>
</html>
```

### More Text Elements\_ Lists

```html
<!DOCTYPE html>
<html>
  <head>
    <title>basic language of the web:HTML</title>
  </head>
  <body>
    <h1>📘 The Code Magazine</h1>
    <h2>The Basic Language of the Web: HTML</h2>

    <p>Posted by <strong>Laura Jones</strong> on Monday, June 21st 2027</p>

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
      HTML stands for <strong>H</strong>yperText <strong>M</strong>arkup
      <strong>L</strong>anguage. It's a markup language that web developers use
      to structure and describe the content of a webpage (not a programming
      language).
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
      <li>You can learn more at the MDN Web Docs.</li>
    </ol>
    <h3>Why should you learn HTML?</h3>
    <p>
      There are countless reasons for learning the fundamental language of the
      web. Here are 5 of them:
    </p>
    <ul>
      <li>
        To be able to use the fundamental web dev language To hand-craft
        beautiful
      </li>
      <li>
        websites instead of relying on tools like Worpress or Wix To build web
      </li>
      <li>applications To impress friends</li>
      <li>To have fun 😃</li>
    </ul>
    <p>Hopefully you learned something new here. See you next time!</p>
  </body>
</html>
```

### Images and Attributes

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>basic language of the web:HTML</title>
  </head>
  <body>
    <h1>📘 The Code Magazine</h1>
    <h2>The Basic Language of the Web: HTML</h2>
    <img
      src="./laura-jones.jpg"
      width="50"
      height="50"
      alt="Head shot of lara jones"
    />
    <p>Posted by <strong>Laura Jones</strong> on Monday, June 21st 2027</p>
    <img
      src="./post-img.jpg"
      alt="html code on a screen"
      width="500"
      height="200"
    />
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
      HTML stands for <strong>H</strong>yperText <strong>M</strong>arkup
      <strong>L</strong>anguage. It's a markup language that web developers use
      to structure and describe the content of a webpage (not a programming
      language).
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
      <li>You can learn more at the MDN Web Docs.</li>
    </ol>
    <h3>Why should you learn HTML?</h3>
    <p>
      There are countless reasons for learning the fundamental language of the
      web. Here are 5 of them:
    </p>
    <ul>
      <li>
        To be able to use the fundamental web dev language To hand-craft
        beautiful
      </li>
      <li>
        websites instead of relying on tools like Worpress or Wix To build web
      </li>
      <li>applications To impress friends</li>
      <li>To have fun 😃</li>
    </ul>
    <p>Hopefully you learned something new here. See you next time!</p>
  </body>
</html>
```

**output**
![](../images/8.png)

### Hyperlinks

```html
<a href="blog.html">Blog</a>
<a href="#">Challenges</a>
<a href="#">FlexBox</a>
<a href="#">Css Grid</a>
```

### Structuring our Page

using **article,header,nav,footer**

---

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>basic language of the web:HTML</title>
  </head>
  <body>
    <header>
      <h1>📘 The Code Magazine</h1>
      <nav>
        <a href="blog.html">Blog</a>
        <a href="#">Challenges</a>
        <a href="#">FlexBox</a>
        <a href="#">Css Grid</a>
      </nav>
    </header>
    <article>
      <header>
        <h2>The Basic Language of the Web: HTML</h2>
        <img
          src="./laura-jones.jpg"
          width="50"
          height="50"
          alt="Head shot of lara jones"
        />
        <p>Posted by <strong>Laura Jones</strong> on Monday, June 21st 2027</p>
        <img
          src="./post-img.jpg"
          alt="html code on a screen"
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
        HTML stands for <strong>H</strong>yperText <strong>M</strong>arkup
        <strong>L</strong>anguage. It's a markup language that web developers
        use to structure and describe the content of a webpage (not a
        programming language).
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
        <li>You can learn more at the MDN Web Docs.</li>
      </ol>
      <h3>Why should you learn HTML?</h3>
      <p>
        There are countless reasons for learning the fundamental language of the
        web. Here are 5 of them:
      </p>
      <ul>
        <li>
          To be able to use the fundamental web dev language To hand-craft
          beautiful
        </li>
        <li>
          websites instead of relying on tools like Worpress or Wix To build web
        </li>
        <li>applications To impress friends</li>
        <li>To have fun 😃</li>
      </ul>
      <p>
        You can learn more at
        <a
          target="_blank"
          href="https://developer.mozilla.org/en-US/docs/Web/HTML"
          >MDN Web Docs</a
        >.
      </p>

      <p>Hopefully you learned something new here. See you next time!</p>
    </article>
    <footer>Copyright &copy; 2022 The Code Magazine</footer>
  </body>
</html>
```

### A Note on Semantic HTML

importance of semantic html

- better SEO
- accessibility

### CHALLENGE #1

```html
<aside>
  <h2>Relates posts</h2>
  <ul>
    <li>
      <img
        src="./images/related-1.jpg"
        width="75"
        height="75"
        alt="man typing on a laptop"
      />
      <a href="#">How to learn web development</a>
      <p>By Chamara Weerasinghe</p>
    </li>
    <li>
      <img
        src="./images/related-2.jpg"
        width="75"
        he
        alt="man typing on a laptop"
      />
      <a href="#">How to learn web development</a>
      <p>By Shan Dinesh</p>
    </li>
    <li>
      <img
        src="./images/related-3.jpg"
        width="75"
        he
        alt="man typing on a laptop"
      />
      <a href="#">How to learn web development</a>
      <p>By Gagani Dharika</p>
    </li>
  </ul>
</aside>
```

output

![](../images/9.png)

### CHALLENGE #2

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Side Project</title>
</head>
<body>
  <aticle>
    <header>
      <h1>
        Converse Chuck Taylor All Star Low Top
      </h1>
      <img src="https://images.unsplash.com/photo-1606107557195-0e29a4b5b4aa?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=764&q=80"  height="400" alt="">
    </header>
    <p><strong>$ 65.00</strong></p>
    <p>Freen Shipping</p>
    <p>Ready to dress up or down. these classic canvas chuks are an every day staple</p>
    <a href="#">More Information &rarr;</a>
    <h2>Product Details</h2>
    <ul>
      <li>Lightweight, durable canvas sneaker</li>
      <li>Lightyt padded footbed for added comfort</li>
      <li>Iconic chuck taylor ankle patch</li>
    </ul>
    <button>Add to cart</button>
    </article>
</body>
</html>

```

**output**
![](../images/10.png)
