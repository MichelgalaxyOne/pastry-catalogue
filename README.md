# Pastry Catalogue

A small static front-end project: an interactive **cake catalogue** with an animated carousel, plus a photo gallery page. Built with plain HTML, CSS and JavaScript, no framework and no build step.

## Demo

- **Live demo:** https://michelgalaxyone.github.io/pastry-catalogue/

## Features

- **Cake carousel** (`index.html`): cakes slide in a stack; the previous / next buttons rotate the items and animate the title, description and action button of the active cake.
- **Order fields per cake**: a cake-type checkbox and a quantity input, with an "Ajouter" (Add) button.
- **Photo gallery** (`cat.html`): four cake photos in grayscale that turn to color and widen on hover.

## Tech stack

- HTML5, CSS3 (transitions, keyframe animations, `nth-child` positioning)
- Vanilla JavaScript (DOM manipulation, no dependencies)
- [Font Awesome 6.4.2](https://fontawesome.com) for the navigation icons (loaded from a CDN)

## Getting started

No installation needed. Choose one option:

**Option 1: open the file directly**

Double-click `index.html` (carousel) or `cat.html` (gallery).

**Option 2: local server (recommended)**

```bash
# with Python
python -m http.server 8000

# or place the folder in xampp/htdocs and open http://localhost/catalogue/
```

Then open http://localhost:8000.

> An internet connection is needed to load the Font Awesome icons.

## Project structure

```
catalogue/
├── index.html        Cake carousel
├── cat.html          Photo gallery
├── css/
│   ├── style.css     Carousel styles
│   └── stylecat.css  Gallery styles
├── js/               (empty, the carousel script is currently inline in index.html)
└── img/              Cake photos (1.jpg to 8.jpg)
```

## Roadmap

- [ ] Replace the placeholder text (every slide currently reads "Croustille") with real cake names, descriptions and prices
- [ ] Make "Ajouter" functional (shopping cart and order summary)
- [ ] Move the carousel script into `js/script.js` and give each slide unique form IDs
- [ ] Fix the icon of the "next" button (it currently uses the left arrow)
- [ ] Make the layout responsive (fixed pixel positions for now)
- [ ] Link the gallery page from the carousel and use all 8 photos
- [ ] Add a page title, meta description and alt text for accessibility and SEO
- [ ] Add a backend (order storage and contact form)

## Credits

The carousel layout and animation are adapted from a TikTok tutorial by **@CodeTheWorld**. The cake content, forms and gallery are my own additions.

## Author

**Marie-Michel HOUNKPE**: [GitHub @MichelgalaxyOne](https://github.com/MichelgalaxyOne)

## License

Released under the MIT license (add a `LICENSE` file to confirm).
