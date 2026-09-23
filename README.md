<p align="center">
 <strong>FalloutLoading</strong><br/>
 A lightweight Fallout: New Vegas-inspired loading page built for browser and game-server loading screens.<br/>
 Features a custom animated radar indicator, Mojave styling, and automatically rotating server hints.<br/>
</p>

<p align="center">
 <a href="https://bleonheart.github.io/FalloutLoading/">
  <img src="https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue?logo=github" alt="Live Demo" />
 </a>
</p>

<h1 align="center">FalloutLoading</h1>

---

## Live Demo

<p align="center">
 <a href="https://bleonheart.github.io/FalloutLoading/">https://bleonheart.github.io/FalloutLoading/</a>
</p>

## Overview

FalloutLoading is a small static loading-screen project themed around Fallout: New Vegas.

It uses plain HTML, CSS, and a small amount of JavaScript to provide an animated loading experience without a build system or backend.

## Features

- Fallout-inspired orange-on-dark visual style
- Animated radar/loading indicator
- Rotating server hints
- Smooth hint fade transitions
- Responsive layout
- Google Fonts integration
- No build step
- No server-side dependencies
- GitHub Pages compatible

## Quick Start

Clone the repository:

```bash
git clone https://github.com/bleonheart/FalloutLoading.git
cd FalloutLoading
```

Open `index.html` directly or serve it locally:

```bash
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## Customization

### Loading Hints

Hints are defined in the `hints` array inside `index.html`.

```javascript
var hints = [
  "Your first loading message",
  "Your second loading message",
  "Your third loading message"
];
```

The page automatically cycles through the entries.

To change the interval, edit the value passed to:

```javascript
setInterval(cycleHints, 3000);
```

The value is measured in milliseconds.

### Styling

Most visual customization lives in `style.css`.

The current theme uses:

- Dark background
- Fallout-style orange accent color
- Animated circular radar effect
- Large centered hint panel

Changing the accent color in the stylesheet is enough to quickly retheme most of the page.

## Repository Structure

```text
FalloutLoading/
├── index.html
└── style.css
```

## Hosting

The project is fully static and can be deployed through:

- GitHub Pages
- Nginx
- Apache
- Any static web host
- A Garry's Mod loading-screen URL

## Contributing

Improvements to the layout, responsiveness, animation, accessibility, or customization options are welcome.

1. Fork the repository
2. Create a feature branch
3. Make and test your changes
4. Open a pull request describing the improvement
