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

### The 7 Steps to a Great Website

![](./images/1.png)
![](./images/2.png)
![](./images/3.png)
![](./images/4.png)
![](./images/5.png)
![](./images/6.png)
![](./images/7.png)

### Defining and Planning the Project (Steps 1 and 2)

![](./images/8.png)
![](./images/9.png)
![](./images/10.png)

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

![](./images/11.png)

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
![](./images/12.png)

### Responsive Design Principles

![](./images/13.png)
![](./images/14.png)
![](./images/15.png)

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

**output**

![](./images/16.png)
![](./images/17.png)

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

**html**

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
![](./images/18.png)

### Building the Hero - Part 2/3

![](./images/20.png)

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

![](./images/19.png)

### Building the Header

### Building the Navigation

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

![](./images/21.png)
![](./images/22.png)
![](./images/23.png)
![](./images/24.png)
![](./images/25.png)
![](./images/26.png)
![](./images/27.png)
![](./images/28.png)
![](./images/29.png)
![](./images/30.png)
![](./images/31.png)
![](./images/32.png)
![](./images/33.png)
![](./images/34.png)
![](./images/35.png)
![](./images/36.png)
![](./images/37.png)
![](./images/38.png)
![](./images/39.png)
![](./images/40.png)
![](./images/41.png)
![](./images/42.png)
![](./images/43.png)
![](./images/44.png)
![](./images/45.png)
![](./images/46.png)
![](./images/47.png)
![](./images/48.png)
![](./images/49.png)
![](./images/50.png)
![](./images/51.png)
![](./images/52.png)
![](./images/53.png)
![](./images/54.png)
![](./images/55.png)
![](./images/56.png)
![](./images/57.png)
![](./images/58.png)
![](./images/59.png)
![](./images/60.png)
![](./images/61.png)
![](./images/62.png)
![](./images/63.png)
![](./images/64.png)
![](./images/65.png)
![](./images/66.png)
![](./images/67.png)
![](./images/68.png)
![](./images/69.png)
![](./images/70.png)
![](./images/71.png)
![](./images/72.png)
![](./images/73.png)
![](./images/74.png)
![](./images/75.png)
![](./images/76.png)
![](./images/77.png)
![](./images/78.png)
![](./images/79.png)
![](./images/80.png)
![](./images/81.png)
![](./images/82.png)
![](./images/83.png)
![](./images/84.png)
![](./images/85.png)
![](./images/86.png)
![](./images/87.png)
![](./images/88.png)
![](./images/89.png)
![](./images/90.png)
![](./images/91.png)
![](./images/92.png)
![](./images/93.png)
![](./images/94.png)
![](./images/95.png)
![](./images/96.png)
![](./images/97.png)
![](./images/98.png)
![](./images/99.png)
![](./images/100.png)
![](./images/101.png)
![](./images/102.png)
![](./images/103.png)
![](./images/104.png)
![](./images/105.png)
![](./images/106.png)
![](./images/107.png)
![](./images/108.png)
![](./images/109.png)
![](./images/110.png)
