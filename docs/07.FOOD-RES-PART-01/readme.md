# Food Restaurant Part 1 🏠

- [Food Restaurant Part 1](../../README.md)
  - [The 7 Steps to a Great Website](#the-7-steps-to-a-great-website)
  - [Defining and Planning the Project (Steps 1 and 2)](#defining-and-planning-the-project-steps-1-and-2)
    - [sections](#sections)
  - [Sketching Initial Layout Ideas (Step 3)](#sketching-initial-layout-ideas-step-3)
  - [First Design and Development Steps (Step 4)](#first-design-and-development-steps-step-4)
  - [Responsive Design Principles](#responsive-design-principles)
  - [How rem and max-width Work](#how-rem-and-max-width-work)
  - [Building the Hero - Part 1](#building-the-hero---part-1)
  - [Building the Hero - Part 2/3](#building-the-hero---part-23)
  - [Building the Header](#building-the-header)
  - [Building the Navigation](#building-the-navigation)
  - [Setting Up a Reusable Grid](#setting-up-a-reusable-grid)
  - [Building the How-It-Works Section - Part 1](#building-the-how-it-works-section---part-1)
  - [Building the How-It-Works Section - Part 2](#building-the-how-it-works-section---part-2)
  - [Building the Featured-In Section](#building-the-featured-in-section)
  - [Building the Meals Section - Part 1](#building-the-meals-section---part-1)
  - [Building the Meals Section - Part 2](#building-the-meals-section---part-2)
  - [Building the Meals Section - Part 3](#building-the-meals-section---part-3)
  - [Building the Testimonials Section - Part 1](#building-the-testimonials-section---part-1)
  - [Building the Testimonials Section - Part 2](#building-the-testimonials-section---part-2)
  - [Building the Pricing Section - Part 1](#building-the-pricing-section---part-1)
  - [Building the Pricing Section - Part 2](#building-the-pricing-section---part-2)
  - [Building the Features Part](#building-the-features-part)
  - [Building the Call-To-Action Section - Part 1](#building-the-call-to-action-section---part-1)
  - [Building the Call-To-Action Section - Part 2](#building-the-call-to-action-section---part-2)
  - [Building the Call-To-Action Section - Part 3](#building-the-call-to-action-section---part-3)
  - [Building the Footer - Part 1](#building-the-footer---part-1)
  - [Building the Footer - Part 2](#building-the-footer---part-2)

## The 7 Steps to a Great Website

![img](./images/1.png)
![img](./images/2.png)
![img](./images/3.png)
![img](./images/4.png)
![img](./images/5.png)
![img](./images/6.png)
![img](./images/7.png)

### Defining and Planning the Project (Steps 1 and 2)

![img](./images/8.png)
![img](./images/9.png)
![img](./images/10.png)

#### sections

- Logo + Navigation
- Hero
- Featured in
- How it works
- Meals(list of diets)
- Testimonials + Gallery
- Pricing + Features
- CTA
- Footer

### Sketching Initial Layout Ideas (Step 3)

![img](./images/11.png)

### First Design and Development Steps (Step 4)

```css
/* 
-- 01 TYPOGRAPHY SYSTEM
-- ---------------------------------------------------------
- FONT SIZE SYSTEM (px)
10 / 12 / 14 / 16 / 18 / 20 / 24 / 30 / 36 / 44 / 52 / 62 / 74 / 86 / 98

- FONT WEIGHT SYSTEM
Default: 400

- LINE HEIGHT SYSTEM (px)
Default:1


-- 02 COLORS SYSTEM

- PRIMARY COLOR : #e67e22
- TINTS:
- SHADES:
- ACCENTS:
- GRAYS:
#555

--- 05 SHADOWS 
--- 06 BORDER RADIUS
--- 07 WHITE SPACE
- SPACING SYSTEM (px)
2 / 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 80 / 96 / 128


      
*/

/* global reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: sans-serif;
  line-height: 1;
  font-weight: 400;
  color: #555;
}
```

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="./css/style.css" />
    <title>Omini Food</title>
  </head>
  <body>
    <h1>A healthy meal delivered to your door, every single day</h1>
  </body>
</html>
```

**output**
![img](./images/12.png)

### Responsive Design Principles

![img](./images/13.png)
![img](./images/14.png)
![img](./images/15.png)

### How rem and max-width Work

```css
/* 
-- 01 TYPOGRAPHY SYSTEM
-- ---------------------------------------------------------
- FONT SIZE SYSTEM (px)
10 / 12 / 14 / 16 / 18 / 20 / 24 / 30 / 36 / 44 / 52 / 62 / 74 / 86 / 98

- FONT WEIGHT SYSTEM
Default: 400

- LINE HEIGHT SYSTEM (px)
Default:1


-- 02 COLORS SYSTEM

- PRIMARY COLOR : #e67e22
- TINTS:
- SHADES:
- ACCENTS:
- GRAYS:
#555

--- 05 SHADOWS 
--- 06 BORDER RADIUS
--- 07 WHITE SPACE
- SPACING SYSTEM (px)
2 / 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 80 / 96 / 128


      
*/

/* global reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  /* font-size: 10px; */
  /* 
  10/16*100 = 62.5%
  */
  font-size: 62.5%;
}

body {
  font-family: sans-serif;
  line-height: 1;
  font-weight: 400;
  color: #555;
}

.test {
  max-width: 50rem;
  background-color: red;
  padding: 4rem;
  font-size: 2rem;
  /* width: 1000px; */
}
```

#### **output**

![img](./images/16.png)
![img](./images/17.png)

### Building the Hero - Part 1

```css
/* 
-- 01 TYPOGRAPHY SYSTEM
-- ---------------------------------------------------------
- FONT SIZE SYSTEM (px)
10 / 12 / 14 / 16 / 18 / 20 / 24 / 30 / 36 / 44 / 52 / 62 / 74 / 86 / 98

- FONT WEIGHT SYSTEM
Default: 400

- LINE HEIGHT SYSTEM (px)
Default:1


-- 02 COLORS SYSTEM

- PRIMARY COLOR : #e67e22
- TINTS:
- SHADES:
- ACCENTS:
- GRAYS:
#555

--- 05 SHADOWS 
--- 06 BORDER RADIUS
--- 07 WHITE SPACE
- SPACING SYSTEM (px)
2 / 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 80 / 96 / 128


      
*/

/* global reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  /* font-size: 10px; */
  /* 
  10/16*100 = 62.5%
  */
  font-size: 62.5%;
}

body {
  font-family: sans-serif;
  line-height: 1;
  font-weight: 400;
  color: #555;
}
.hero {
  max-width: 130rem;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr 1fr;
}
.hero-img {
  width: 100%;
}
```

#### html

```html
<section class="section-hero">
  <div class="hero">
    <div class="hero-text-box">
      <h1 class="heading-primary">
        A healthy meal delivered to your door, every single day
      </h1>
      <div class="hero-description">
        The smart 365-days-per-year food subscription that will make you eat
        healthy again. Tailored to your personal tastes and nutritional needs.
        We have delivered 250,000+ meals last year!
      </div>
      <a class="btn " href="#">start eating well</a>
      <a class="btn " href="#">Learn more &darr;</a>
    </div>
    <div class="hero-img-box">
      <img
        src="./img/hero.png"
        alt="different type of food in dishes"
        class="hero-img"
      />
    </div>
  </div>
</section>
```

**output**
![img](./images/18.png)

### Building the Hero - Part 2/3

![img](./images/20.png)

```css
/* 
-- 01 TYPOGRAPHY SYSTEM
-- ---------------------------------------------------------
- FONT SIZE SYSTEM (px)
10 / 12 / 14 / 16 / 18 / 20 / 24 / 30 / 36 / 44 / 52 / 62 / 74 / 86 / 98

- FONT WEIGHT SYSTEM
Default: 400

- LINE HEIGHT SYSTEM (px)
Default:1


-- 02 COLORS SYSTEM

- PRIMARY COLOR : #e67e22
- TINTS:#fdf2e9
- SHADES: #cf711f 
- ACCENTS:
- GRAYS:
#555
#333

--- 05 SHADOWS 
--- 06 BORDER RADIUS
--- 07 WHITE SPACE
- SPACING SYSTEM (px)
2 / 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 80 / 96 / 128


      
*/

/* global reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  /* font-size: 10px; */
  /* 
  10/16*100 = 62.5%
  */
  font-size: 62.5%;
}

body {
  font-family: 'Rubik', sans-serif;
  line-height: 1;
  font-weight: 400;
  color: #555;
}
.section-hero {
  padding: 9.6rem 0;
  background-color: #fdf2e9;
}

.hero {
  max-width: 130rem;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 9.6rem;
  align-items: center;
}
.hero-img {
  width: 100%;
}

.hero-text-box {
}
.heading-primary {
  font-size: 5.2rem;
  font-weight: 700;
  line-height: 1.05;
  color: #333;
  letter-spacing: -0.5px;
  margin-bottom: 3.2rem;
}
.hero-description {
  font-size: 2rem;
  line-height: 1.6;
  color: #555;
  margin-bottom: 4.8rem;
}

.btn:link,
.btn:visited {
  display: inline-block;
  font-size: 2rem;
  padding: 1.6rem 3.2rem;
  font-weight: 600;
  border-radius: 0.9rem;

  text-decoration: none;
}
/* 
.btn:active,
.btn:hover {
  background-color: #e67e22;
  color: #fff;
} */

.btn.btn--outline:link,
.btn.btn--outline:active {
  background-color: #fff;
  color: #555;
}

.btn.btn--outline:hover,
.btn.btn--outline:visited {
  background-color: #fdf2e9;
  color: #555;
  /* border: 3px solid red; */
  /* trick to add box shadow to the inside */
  box-shadow: inset 0 0 0 3px #fff;
}

.btn.btn--full:link,
.btn.btn--full:visited {
  background-color: #e67e22;
  color: #fff;
  transition: background-color 0.2s ease-in-out;
}
.btn.btn--full:hover,
.btn.btn--full:active {
  background-color: #cf711f;
}

.margin-right-sm {
  margin-right: 1.6rem !important;
}

.delivered-meals {
  display: flex;
  /* flex-direction: column; */
  gap: 1rem;
  align-items: center;
  margin-top: 8rem;
}
.delivered-imgs {
  display: flex;
}
.delivered-imgs img {
  height: 4.8rem;
  width: 4.8rem;
  border-radius: 50%;
  margin-right: -1.6rem;
  border: 3px solid #fdf2e9;
}

.delivered-imgs img:last-child {
  margin-right: 0;
}
.delivered-text {
  font-size: 1.8rem;
  font-weight: 600;
}
.delivered-text span {
  color: #cf711f;
  font-weight: 700;
}
```

html

```html
<section class="section-hero">
  <div class="hero">
    <div class="hero-text-box">
      <h1 class="heading-primary">
        A healthy meal delivered to your door, every single day
      </h1>
      <div class="hero-description">
        The smart 365-days-per-year food subscription that will make you eat
        healthy again. Tailored to your personal tastes and nutritional needs.
      </div>
      <a class="btn btn--full margin-right-sm" href="#">start eating well</a>
      <a class="btn btn--outline" href="#">Learn more &darr;</a>
      <div class="delivered-meals">
        <div class="delivered-imgs">
          <img src="./img/customers/customer-1.jpg" alt="customers" />
          <img src="./img/customers/customer-2.jpg" alt="customers" />
          <img src="./img/customers/customer-3.jpg" alt="customers" />
          <img src="./img/customers/customer-4.jpg" alt="customers" />
          <img src="./img/customers/customer-5.jpg" alt="customers" />
          <img src="./img/customers/customer-6.jpg" alt="customers" />
        </div>
        <p class="delivered-text">
          <span>250,000+ </span> meals delivered last year!
        </p>
      </div>
    </div>
    <div class="hero-img-box">
      <img
        src="./img/hero.png"
        alt="different type of food in dishes"
        class="hero-img"
      />
    </div>
  </div>
</section>
```

output

![img](./images/19.png)

### Building the Header

let's add the header markup

```html
  <body>
    <header class="header">
      <img
        class="logo"
        src="./img/omnifood-logo.png"
        alt="omniFood logo"
      />
      <nav class="main-nav">Navigation</nav>
    </header>
```

and put the section inside the main element.

```html
<main>
  <section>
    ....
  </section>
</main>
```

we use `<main>` element to wrap the main content of the page.

let's restructure the code to make it more readable

```css
/* 
-- 01 TYPOGRAPHY SYSTEM
-- ---------------------------------------------------------
- FONT SIZE SYSTEM (px)
10 / 12 / 14 / 16 / 18 / 20 / 24 / 30 / 36 / 44 / 52 / 62 / 74 / 86 / 98

- FONT WEIGHT SYSTEM
Default: 400

- LINE HEIGHT SYSTEM (px)
Default:1


-- 02 COLORS SYSTEM

- PRIMARY COLOR : #e67e22
- TINTS:#fdf2e9
- SHADES: #cf711f 
- ACCENTS:
- GRAYS:
#555
#333

--- 05 SHADOWS 
--- 06 BORDER RADIUS
--- 07 WHITE SPACE
- SPACING SYSTEM (px)
2 / 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 80 / 96 / 128


      
*/

/* global reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  /* font-size: 10px; */
  /* 
  10/16*100 = 62.5%
  */
  font-size: 62.5%;
}

body {
  font-family: 'Rubik', sans-serif;
  line-height: 1;
  font-weight: 400;
  color: #555;
}

/* ************************************** */
/* GENERAL REUSABLE COMPONENTS */
.heading-primary {
  font-size: 5.2rem;
  font-weight: 700;
  line-height: 1.05;
  color: #333;
  letter-spacing: -0.5px;
  margin-bottom: 3.2rem;
}

.btn:link,
.btn:visited {
  display: inline-block;
  font-size: 2rem;
  padding: 1.6rem 3.2rem;
  font-weight: 600;
  border-radius: 0.9rem;

  text-decoration: none;
}
/* 
.btn:active,
.btn:hover {
  background-color: #e67e22;
  color: #fff;
} */

.btn.btn--outline:link,
.btn.btn--outline:active {
  background-color: #fff;
  color: #555;
}

.btn.btn--outline:hover,
.btn.btn--outline:visited {
  background-color: #fdf2e9;
  color: #555;
  /* border: 3px solid red; */
  /* trick to add box shadow to the inside */
  box-shadow: inset 0 0 0 3px #fff;
}

.btn.btn--full:link,
.btn.btn--full:visited {
  background-color: #e67e22;
  color: #fff;
  transition: background-color 0.2s ease-in-out;
}
.btn.btn--full:hover,
.btn.btn--full:active {
  background-color: #cf711f;
}

.margin-right-sm {
  margin-right: 1.6rem !important;
}

/* ************************************** */
/* HEADER SECTION */
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #fdf2e9;
  /* because we want header to be sticky later */
  height: 9.6rem;
  padding: 0 4.8rem;
}
.logo {
  height: 2.2rem;
}

/* ************************************** */
/* HERO SECTION */

.section-hero {
  padding: 4.8rem 0 9.6rem 0;
  background-color: #fdf2e9;
}

.hero {
  max-width: 130rem;
  margin: 0 auto;
  padding: 0 3.2rem;
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 9.6rem;
  align-items: center;
}
.hero-img {
  width: 100%;
}

.hero-text-box {
}

.hero-description {
  font-size: 2rem;
  line-height: 1.6;
  color: #555;
  margin-bottom: 4.8rem;
}

.delivered-meals {
  display: flex;
  /* flex-direction: column; */
  gap: 1rem;
  align-items: center;
  margin-top: 8rem;
}
.delivered-imgs {
  display: flex;
}
.delivered-imgs img {
  height: 4.8rem;
  width: 4.8rem;
  border-radius: 50%;
  margin-right: -1.6rem;
  border: 3px solid #fdf2e9;
}

.delivered-imgs img:last-child {
  margin-right: 0;
}
.delivered-text {
  font-size: 1.8rem;
  font-weight: 600;
}
.delivered-text span {
  color: #cf711f;
  font-weight: 700;
}

```

output

![img](./images/21.png)

### Building the Navigation

adding the navigation markup

```html
### Setting Up a Reusable Grid

### Building the How-It-Works Section - Part 1

### Building the How-It-Works Section - Part 2

### Building the Featured-In Section

### Building the Meals Section - Part 1

### Building the Meals Section - Part 2

### Building the Meals Section - Part 3

### Building the Testimonials Section - Part 1

### Building the Testimonials Section - Part 2

### Building the Pricing Section - Part 1

### Building the Pricing Section - Part 2

### Building the Features Part

### Building the Call-To-Action Section - Part 1

### Building the Call-To-Action Section - Part 2

### Building the Call-To-Action Section - Part 3

### Building the Footer - Part 1

### Building the Footer - Part 2

![img](./images/21.png)
![img](./images/22.png)
![img](./images/23.png)
![img](./images/24.png)
![img](./images/25.png)
![img](./images/26.png)
![img](./images/27.png)
![img](./images/28.png)
![img](./images/29.png)
![img](./images/30.png)
![img](./images/31.png)
![img](./images/32.png)
![img](./images/33.png)
![img](./images/34.png)
![img](./images/35.png)
![img](./images/36.png)
![img](./images/37.png)
![img](./images/38.png)
![img](./images/39.png)
![img](./images/40.png)
![img](./images/41.png)
![img](./images/42.png)
![img](./images/43.png)
![img](./images/44.png)
![img](./images/45.png)
![img](./images/46.png)
![img](./images/47.png)
![img](./images/48.png)
![img](./images/49.png)
![img](./images/50.png)
![img](./images/51.png)
![img](./images/52.png)
![img](./images/53.png)
![img](./images/54.png)
![img](./images/55.png)
![img](./images/56.png)
![img](./images/57.png)
![img](./images/58.png)
![img](./images/59.png)
![img](./images/60.png)
![img](./images/61.png)
![img](./images/62.png)
![img](./images/63.png)
![img](./images/64.png)
![img](./images/65.png)
![img](./images/66.png)
![img](./images/67.png)
![img](./images/68.png)
![img](./images/69.png)
![img](./images/70.png)
![img](./images/71.png)
![img](./images/72.png)
![img](./images/73.png)
![img](./images/74.png)
![img](./images/75.png)
![img](./images/76.png)
![img](./images/77.png)
![img](./images/78.png)
![img](./images/79.png)
![img](./images/80.png)
![img](./images/81.png)
![img](./images/82.png)
![img](./images/83.png)
![img](./images/84.png)
![img](./images/85.png)
![img](./images/86.png)
![img](./images/87.png)
![img](./images/88.png)
![img](./images/89.png)
![img](./images/90.png)
![img](./images/91.png)
![img](./images/92.png)
![img](./images/93.png)
![img](./images/94.png)
![img](./images/95.png)
![img](./images/96.png)
![img](./images/97.png)
![img](./images/98.png)
![img](./images/99.png)
![img](./images/100.png)
![img](./images/101.png)
![img](./images/102.png)
![img](./images/103.png)
![img](./images/104.png)
![img](./images/105.png)
![img](./images/106.png)
![img](./images/107.png)
![img](./images/108.png)
![img](./images/109.png)
![img](./images/110.png)
