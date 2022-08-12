# Home Page

- [Home Page](#home-page)
  - [How Media Queries Work](#how-media-queries-work)
    - [Adding test media queries](#adding-test-media-queries)
  - [How to Select Breakpoints](#how-to-select-breakpoints)
  - [Responding to Small Laptops](#responding-to-small-laptops)
  - [Responding to Landscape Tablets](#responding-to-landscape-tablets)
    - [adding queries.css file](#adding-queriescss-file)
    - [Adding media queries](#adding-media-queries)
  - [Responding to Tablets](#responding-to-tablets)
    - [Adding media queries for tablets](#adding-media-queries-for-tablets)
  - [Building the Mobile Navigation](#building-the-mobile-navigation)
  - [Responding to Smaller Tablets](#responding-to-smaller-tablets)
  - [Responding to Phones](#responding-to-phones)

## How Media Queries Work

![image](images/1.png)

### Adding test media queries

```css
/**************************/
/* HERO SECTION */
/**************************/

.section-hero {
  background-color: #fdf2e9;
  padding: 4.8rem 0 9.6rem 0;
}

@media (max-width: 1200px) {
  .section-hero {
    background-color: orangered;
  }
}

@media (max-width: 600px) {
  .section-hero {
    border: 20px solid blue;
    background-color: blue;
  }
}
```

![image](images/2.png)

![image](images/3.png)

## How to Select Breakpoints

![image](images/4.png)

## Responding to Small Laptops

this is very important for responsive design

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

## Responding to Landscape Tablets

### adding queries.css file

```html
<link rel="stylesheet" href="css/queries.css" />
```

### Adding media queries

```css
/* rem and em do not depend on font size in media queries
instead 1rem = 1em = 16px 
*/

/* ***************************************** */
/* BELOW 1344 px (SMALLER DESKTOPS) */
@media (max-width: 84em) {
  .hero {
    max-width: 120rem;
  }

  .heading-primary {
    font-size: 4.4rem;
  }

  .gallery {
    grid-template-columns: repeat(2, 1fr);
  }
}

/* ***************************************** */
/* BELOW 1200 px (landscape tablets) */

@media (max-width: 75em) {
  html {
    /* 9/16*100 */
    font-size: 56.25%;
  }

  .grid {
    column-gap: 4.8rem;
    row-gap: 6.4rem;
  }
  .heading-secondary {
    font-size: 3.6rem;
  }

  .heading-tertiary {
    font-size: 2.4rem;
  }
  .header {
    padding: 0 3.2rem;
  }
  .hero {
    gap: 4.8rem;
  }

  .main-nav-list {
    gap: 3.2rem;
  }
  .testimonials-container {
    padding: 4.8rem;
  }
}

/* 

- Font sizes (px)
10 / 12 / 14 / 16 / 18 / 20 / 24 / 30 / 36 / 44 / 52 / 62 / 74 / 86 / 98 */
```

and add this to the stye file

```css
.main-nav-list {
  list-style: none;
  display: flex;
  align-items: center;
  gap: 4.8rem;
}
```

## Responding to Tablets

### Adding media queries for tablets

```css
.list-item {
  font-size: 1.8rem;
  display: flex;
  align-items: center;
  gap: 1.6rem;
  line-height: 1.2;
}

/* ***************************************** */
/* BELOW 940 px (tablets) */

@media (max-width: 59em) {
  html {
    /* 8/16*100 */
    font-size: 50%;
  }
  .hero {
    grid-template-columns: 1fr;
    padding: 0 8 rem;
    gap: 6.4rem;
  }

  .hero-img {
    width: 60%;
  }
  .hero-text-box,
  .hero-img-box {
    text-align: center;
  }
  .delivered-meals {
    justify-content: center;
    margin-top: 3.2rem;
  }
  .logos img {
    height: 2.4rem;
  }

  .step-number {
    font-size: 7.4rem;
  }
  .meal-content {
    padding: 2.4rem 3.2rem 3.2rem 3.2rem;
  }
  .section-testimonials {
    grid-template-columns: 1fr;
  }
  .gallery {
    grid-template-columns: repeat(6, 1fr);
  }
  .cta {
    grid-template-columns: 3fr 2fr;
  }
  .cta-form {
    grid-template-columns: 1fr;
  }
  .btn--form {
    margin-top: 1.2rem;
  }
}
/* 

- Font sizes (px)
10 / 12 / 14 / 16 / 18 / 20 / 24 / 30 / 36 / 44 / 52 / 62 / 74 / 86 / 98 */

/* --- 07 WHITESPACE

- Spacing system (px)
2 / 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 80 / 96 / 128
 
*/
```

## Building the Mobile Navigation

## Responding to Smaller Tablets

## Responding to Phones

```

```
