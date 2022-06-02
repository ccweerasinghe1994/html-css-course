- [🥶 Web Design Rules #10 - Part 1\_ Elements and Components](#-web-design-rules-10---part-1_-elements-and-components)
- [👽 Building an Accordion Component - Part 1](#-building-an-accordion-component---part-1)
- [👿 Building an Accordion Component - Part 2](#-building-an-accordion-component---part-2)
- [🔥 Building a Carousel Component - Part 1](#-building-a-carousel-component---part-1)
- [🤡 Building a Carousel Component - Part 2](#-building-a-carousel-component---part-2)
- [🚀 Building a Table Component - Part 1](#-building-a-table-component---part-1)
- [🪨 Building a Table Component - Part 2](#-building-a-table-component---part-2)
- [🤖 CHALLENGE #1\_ Building a Pagination Component](#-challenge-1_-building-a-pagination-component)
- [🧑‍🎤 Web Design Rules #10 - Part 2\_ Layout Patterns](#-web-design-rules-10---part-2_-layout-patterns)
- [🧑‍🚀 Building a Hero Section - Part 1](#-building-a-hero-section---part-1)
- [🎈 Building a Hero Section - Part 2](#-building-a-hero-section---part-2)
- [🧨 Building a Web Application Layout - Part 1](#-building-a-web-application-layout---part-1)
- [🌵 Building a Web Application Layout - Part 2](#-building-a-web-application-layout---part-2)

### 🥶 Web Design Rules #10 - Part 1\_ Elements and Components

![](images/1.png)
![](images/2.png)
![](images/3.png)
![](images/4.png)
![](images/5.png)
![](images/6.png)
![](images/7.png)
![](images/8.png)
![](images/9.png)
![](images/10.png)
![](images/11.png)
![](images/12.png)
![](images/13.png)
![](images/14.png)
![](images/15.png)
![](images/16.png)
![](images/17.png)
![](images/18.png)
![](images/19.png)
![](images/20.png)
![](images/21.png)
![](images/22.png)
![](images/23.png)
![](images/24.png)
![](images/25.png)
![](images/26.png)
![](images/27.png)
![](images/28.png)
![](images/29.png)
![](images/30.png)
![](images/31.png)
![](images/32.png)
![](images/33.png)
![](images/34.png)
![](images/35.png)
![](images/36.png)
![](images/37.png)
![](images/38.png)
![](images/39.png)
![](images/40.png)
![](images/41.png)
![](images/42.png)

### 👽 Building an Accordion Component - Part 1

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link
      href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&display=swap"
      rel="stylesheet"
    />
    <style>
      /*
      SPACING SYSTEM (px)
      2 / 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 80 / 96 / 128

      FONT SIZE SYSTEM (px)
      10 / 12 / 14 / 16 / 18 / 20 / 24 / 30 / 36 / 44 / 52 / 62 / 74 / 86 / 98
      */

      /*
      MAIN COLOR : #087f5b
      GREY COLOR :#343a40

      */

      * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
      }

      /* ------------------------ */
      /* GENERAL STYLES */
      /* ------------------------ */
      body {
        font-family: "Inter", sans-serif;
        color: #343a40;
        line-height: 1;
      }

      .accordion {
        width: 700px;
        margin: 100px auto;
      }
      .item {
      }
      .number,
      .text {
        font-size: 24px;
        font-weight: 500;
        color: #099268;
      }
      .text {
      }
      .icon {
        height: 24px;
        width: 24px;
        stroke: #099268;
      }
      .hidden-box {
      }
      .hidden-box p {
        line-height: 1.6;
        margin-bottom: 24px;
      }

      .hidden-box ul {
        color: #868e96;
        margin-left: 14px;
        display: flex;
        flex-direction: column;
        gap: 12px;
      }
    </style>
    <title>Accordion Component</title>
  </head>
  <body>
    <div class="accordion">
      <div class="item">
        <p class="number">02</p>
        <p class="text">How long do i have to return my chair?</p>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="icon"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M19 9l-7 7-7-7"
          />
        </svg>
        <div class="hidden-box">
          <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quae
            placeat incidunt voluptatibus quidem ipsa similique? Doloremque,
            nihil quibusdam. Fugiat ut nihil porro quo voluptas, ratione quae
            cum cumque molestiae distinctio.
          </p>
          <ul>
            <li>Lorem ipsum dolor sit amet consectetur,</li>
            <li>adipisicing elit. Velit sed voluptatibus,</li>
            <li>totam hic quaerat nihil et illo suscipit quia?</li>
            <li>Quia adipisci doloribus assumenda error impedit?</li>
            <li>Officia necessitatibus ea et doloribus.</li>
          </ul>
        </div>
      </div>
    </div>
  </body>
</html>
```

**output**
![](images/43.png)
![](images/44.png)
**theory**
![](images/45.png)

### 👿 Building an Accordion Component - Part 2

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link
      href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&display=swap"
      rel="stylesheet"
    />
    <style>
      /*
      SPACING SYSTEM (px)
      2 / 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 80 / 96 / 128

      FONT SIZE SYSTEM (px)
      10 / 12 / 14 / 16 / 18 / 20 / 24 / 30 / 36 / 44 / 52 / 62 / 74 / 86 / 98
      */

      /*
      MAIN COLOR : #087f5b
      GREY COLOR :#343a40

      */

      * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
      }

      /* ------------------------ */
      /* GENERAL STYLES */
      /* ------------------------ */
      body {
        font-family: "Inter", sans-serif;
        color: #343a40;
        line-height: 1;
      }

      .accordion {
        width: 700px;
        margin: 100px auto;
        display: flex;
        flex-direction: column;
        gap: 24px;
      }
      .item {
        box-shadow: 0 0 32px rgba(0, 0, 0, 0.1);
        padding: 24px;
        display: grid;
        grid-template-columns: auto 1fr auto;
        column-gap: 24px;
        row-gap: 36px;
        align-items: center;
      }
      .number,
      .text {
        font-size: 24px;
        font-weight: 500;
        /* color: #099268; */
      }

      .number {
        color: #ced4da;
      }
      .text {
      }
      .icon {
        height: 24px;
        width: 24px;
        stroke: #099268;
      }
      .hidden-box {
        grid-column: 2;
        display: none;
      }
      .hidden-box p {
        line-height: 1.6;
        margin-bottom: 24px;
      }

      .hidden-box ul {
        color: #868e96;
        margin-left: 14px;
        display: flex;
        flex-direction: column;
        gap: 12px;
      }

      .open {
        border-top: 4px solid #099268;
      }

      .open .hidden-box {
        display: block;
      }

      .open .icon {
        transform: rotate(180deg);
      }

      .open .text,
      .open .number {
        color: #099268;
      }
    </style>
    <title>Accordion Component</title>
  </head>
  <body>
    <div class="accordion">
      <div class="item">
        <p class="number">01</p>
        <p class="text">Where are the chairs assembled ?</p>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="icon"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M19 9l-7 7-7-7"
          />
        </svg>
        <div class="hidden-box">
          <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quae
            placeat incidunt voluptatibus quidem ipsa similique? Doloremque,
            nihil quibusdam. Fugiat ut nihil porro quo voluptas, ratione quae
          </p>
          <ul>
            <li>Lorem ipsum dolor sit amet consectetur,</li>
            <li>adipisicing elit. Velit sed voluptatibus,</li>
            <li>totam hic quaerat nihil et illo suscipit quia?</li>
            <li>Quia adipisci doloribus assumenda error impedit?</li>
            <li>Officia necessitatibus ea et doloribus.</li>
          </ul>
        </div>
      </div>
      <div class="item open">
        <p class="number">02</p>
        <p class="text">How long do i have to return my chair?</p>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="icon"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M19 9l-7 7-7-7"
          />
        </svg>
        <div class="hidden-box">
          <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quae
            placeat incidunt voluptatibus quidem ipsa similique? Doloremque,
            nihil quibusdam. Fugiat ut nihil porro quo voluptas, ratione quae
          </p>
          <ul>
            <li>Lorem ipsum dolor sit amet consectetur,</li>
            <li>adipisicing elit. Velit sed voluptatibus,</li>
            <li>totam hic quaerat nihil et illo suscipit quia?</li>
            <li>Quia adipisci doloribus assumenda error impedit?</li>
            <li>Officia necessitatibus ea et doloribus.</li>
          </ul>
        </div>
      </div>
      <div class="item">
        <p class="number">03</p>
        <p class="text">Do you ship countries outside EU</p>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="icon"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M19 9l-7 7-7-7"
          />
        </svg>
        <div class="hidden-box">
          <p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quae
            placeat incidunt voluptatibus quidem ipsa similique? Doloremque,
            nihil quibusdam. Fugiat ut nihil porro quo voluptas, ratione quae
          </p>
          <ul>
            <li>Lorem ipsum dolor sit amet consectetur,</li>
            <li>adipisicing elit. Velit sed voluptatibus,</li>
            <li>totam hic quaerat nihil et illo suscipit quia?</li>
            <li>Quia adipisci doloribus assumenda error impedit?</li>
            <li>Officia necessitatibus ea et doloribus.</li>
          </ul>
        </div>
      </div>
    </div>
  </body>
</html>
```

**output**

![](images/46.png)

### 🔥 Building a Carousel Component - Part 1

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link
      href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&display=swap"
      rel="stylesheet"
    />
    <style>
      /*
      SPACING SYSTEM (px)
      2 / 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 80 / 96 / 128

      FONT SIZE SYSTEM (px)
      10 / 12 / 14 / 16 / 18 / 20 / 24 / 30 / 36 / 44 / 52 / 62 / 74 / 86 / 98
      */
      /*
      MAIN COLOR : #087f5b
      GREY COLOR :#343a40

      */

      * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
      }

      /* ------------------------ */
      /* GENERAL STYLES */
      /* ------------------------ */
      body {
        font-family: "Inter", sans-serif;
        color: #343a40;
        line-height: 1;
      }

      .carousel {
        background-color: #087f5b;
        width: 800px;
        margin: 100px auto;
        border-radius: 8px;
        padding: 32px;
        padding-left: 86px;
        display: flex;
        align-items: center;
        gap: 86px;
      }

      img {
        border-radius: 8px;
        height: 200px;
        transform: scale(1.5);
        box-shadow: 0 12px 32px rgba(0, 0, 0, 0.25);
      }
      .testimonial-text {
        font-size: 18px;
        font-weight: 500;
        line-height: 1.5;
        margin-bottom: 32px;
        color: #e6fcf5;
      }
      .testimonial-author {
        font-size: 14px;
        margin-bottom: 4px;
        color: #c3fae8;
      }
      .testimonial-job {
        font-size: 12px;
        color: #c3fae8;
      }
      .button {
      }
      .button-icon {
      }
    </style>
    <title>Accordion Component</title>
  </head>
  <body>
    <div class="carousel">
      <img src="maria.jpg" alt="maria de mel" />
      <blockquote class="testimonial">
        <p class="testimonial-text">
          "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nam nulla
          quia quod cumque unde, et ad minus debitis laborum, distinctio
          necessitatibus ratione eaque expedita. Debitis ullam delectus alias
          temporibus laboriosam!"
        </p>
        <p class="testimonial-author">maria de mel</p>
        <p class="testimonial-job">senior product manager at EDP commercial</p>
      </blockquote>
      <button class="button">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="button-icon"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M15 19l-7-7 7-7"
          />
        </svg>
      </button>
      <button class="button">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="button-icon"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M9 5l7 7-7 7"
          />
        </svg>
      </button>
    </div>
  </body>
</html>
```

output

![](./images/47.png)

### 🤡 Building a Carousel Component - Part 2

### 🚀 Building a Table Component - Part 1

### 🪨 Building a Table Component - Part 2

### 🤖 CHALLENGE #1\_ Building a Pagination Component

### 🧑‍🎤 Web Design Rules #10 - Part 2\_ Layout Patterns

### 🧑‍🚀 Building a Hero Section - Part 1

### 🎈 Building a Hero Section - Part 2

### 🧨 Building a Web Application Layout - Part 1

### 🌵 Building a Web Application Layout - Part 2

![](images/47.png)
![](images/48.png)
![](images/49.png)
![](images/50.png)
![](images/51.png)
![](images/52.png)
![](images/53.png)
![](images/54.png)
![](images/55.png)
![](images/56.png)
![](images/57.png)
![](images/58.png)
![](images/59.png)
![](images/60.png)
![](images/61.png)
![](images/62.png)
![](images/63.png)
![](images/64.png)
![](images/65.png)
![](images/66.png)
![](images/67.png)
![](images/68.png)
![](images/69.png)
![](images/70.png)
![](images/71.png)
![](images/72.png)
![](images/73.png)
![](images/74.png)
![](images/75.png)
![](images/76.png)
![](images/77.png)
![](images/78.png)
![](images/79.png)
![](images/80.png)
![](images/81.png)
![](images/82.png)
![](images/83.png)
![](images/84.png)
![](images/85.png)
![](images/86.png)
![](images/87.png)
![](images/88.png)
![](images/89.png)
![](images/90.png)
![](images/91.png)
![](images/92.png)
![](images/93.png)
![](images/94.png)
![](images/95.png)
![](images/96.png)
![](images/97.png)
![](images/98.png)
![](images/99.png)
![](images/100.png)
![](images/101.png)
![](images/102.png)
![](images/103.png)
![](images/104.png)
![](images/105.png)
![](images/106.png)
![](images/107.png)
![](images/108.png)
![](images/109.png)
![](images/110.png)
![](images/111.png)
![](images/112.png)
![](images/113.png)
![](images/114.png)
![](images/115.png)
![](images/116.png)
![](images/117.png)
![](images/118.png)
![](images/119.png)
![](images/120.png)
![](images/121.png)
![](images/122.png)
![](images/123.png)
![](images/124.png)
![](images/125.png)
![](images/126.png)
![](images/127.png)
![](images/128.png)
![](images/129.png)
![](images/130.png)
![](images/131.png)
![](images/132.png)
![](images/133.png)
![](images/134.png)
![](images/135.png)
![](images/136.png)
![](images/137.png)
![](images/138.png)
![](images/139.png)
![](images/140.png)
![](images/141.png)
![](images/142.png)
![](images/143.png)
![](images/144.png)
![](images/145.png)
![](images/146.png)
![](images/147.png)
![](images/148.png)
![](images/149.png)
![](images/150.png)
![](images/151.png)
![](images/152.png)
![](images/153.png)
![](images/154.png)
![](images/155.png)
![](images/156.png)
![](images/157.png)
![](images/158.png)
![](images/159.png)
![](images/160.png)
![](images/161.png)
![](images/162.png)
![](images/163.png)
![](images/164.png)
![](images/165.png)
![](images/166.png)
![](images/167.png)
![](images/168.png)
![](images/169.png)
![](images/170.png)
![](images/171.png)
![](images/172.png)
![](images/173.png)
![](images/174.png)
![](images/175.png)
![](images/176.png)
![](images/177.png)
![](images/178.png)
![](images/179.png)
![](images/180.png)
![](images/181.png)
![](images/182.png)
![](images/183.png)
![](images/184.png)
![](images/185.png)
![](images/186.png)
![](images/187.png)
![](images/188.png)
![](images/189.png)
![](images/190.png)
![](images/191.png)
![](images/192.png)
![](images/193.png)
![](images/194.png)
![](images/195.png)
![](images/196.png)
![](images/197.png)
![](images/198.png)
![](images/199.png)
![](images/200.png)
![](images/201.png)
![](images/202.png)
![](images/203.png)
![](images/204.png)
![](images/205.png)
![](images/206.png)
![](images/207.png)
![](images/208.png)
![](images/209.png)
![](images/210.png)
![](images/211.png)
![](images/212.png)
![](images/213.png)
![](images/214.png)
![](images/215.png)
![](images/216.png)
![](images/217.png)
![](images/218.png)
![](images/219.png)
![](images/220.png)
![](images/221.png)
![](images/222.png)
![](images/223.png)
![](images/224.png)
![](images/225.png)
![](images/226.png)
![](images/227.png)
![](images/228.png)
![](images/229.png)
