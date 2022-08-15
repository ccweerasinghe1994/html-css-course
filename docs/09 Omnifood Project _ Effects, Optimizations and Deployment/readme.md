# Home Page

## Making the Mobile Navigation Work

### Adding the script file

```html
    </footer>
    <script src="./script.js"></script>
  </body>
```

### Adding js

```js
// MObile Navigation
const btnNavEl = document.querySelector('.btn-mobile-nav');
const headerEl = document.querySelector('.header');

btnNavEl.addEventListener('click', function () {
  headerEl.classList.toggle('nav-open');
});
```

```css
@media (max-width: 59em) {
  /* MOBILE NAVIGATION */
  .btn-mobile-nav {
    display: block;
    z-index: 999;
  }
}
```

### Output

![img](./images/1.png)

## Implementing Smooth Scrolling

## Implementing a Sticky Navigation Bar

### Adding the styles

```css
.sticky .header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 8rem;
  padding-top: 0;
  padding-bottom: 0;
  background-color: rgba(255, 255, 255, 0.97);
  box-shadow: 0 1.2rem 3.6rem rgba(0, 0, 0, 0.03);
  z-index: 10000;
}

.sticky .section-hero {
  margin-top: 9.6rem;
}
```

### Adding the script

```js
// Smooth Scrolling animation

const allLinks = document.querySelectorAll('a:link');

allLinks.forEach(function (link) {
  link.addEventListener('click', function (e) {
    e.preventDefault();
    const target = this.getAttribute('href');

    if (target === '#') {
      window.scroll({
        top: 0,
        behavior: 'smooth',
      });
    }

    if (target !== '#' && target.startsWith('#')) {
      const sectionEl = document.querySelector(target);
      sectionEl.scrollIntoView({ behavior: 'smooth' });
    }

    if (link.classList.contains('main-nav-link')) {
      headerEl.classList.toggle('nav-open');
    }
  });
});

const heroEl = document.querySelector('.section-hero');
// Sticky Navigation
const obs = new IntersectionObserver(
  function (entries) {
    const ent = entries[0];
    if (!ent?.isIntersecting) {
      document.body.classList.add('sticky');
    }
    if (ent?.isIntersecting) {
      document.body.classList.remove('sticky');
    }
  },
  {
    // In the viewPort
    root: null,
    threshold: 0,
    rootMargin: '-80px',
  }
);

obs.observe(heroEl);
```

## Browser Support and Fixing Flexbox Gap in Safari

## Testing Performance With Lighthouse

## Adding Favicon and Meta Description

## Image Optimizations

## Deployment to Netlify

## Making the Form Work With Netlify Forms
