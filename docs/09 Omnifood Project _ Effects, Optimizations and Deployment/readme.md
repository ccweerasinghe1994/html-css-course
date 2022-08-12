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

## Browser Support and Fixing Flexbox Gap in Safari

## Testing Performance With Lighthouse

## Adding Favicon and Meta Description

## Image Optimizations

## Deployment to Netlify

## Making the Form Work With Netlify Forms
