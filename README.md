<p align="center">
 <strong>Ashveil — Mojave-Inspired Loading Screen</strong><br/>
 A lightweight Fallout: New Vegas-inspired loading screen for Garry's Mod servers and static web hosting.<br/>
 Built with plain HTML, CSS, and JavaScript for simple customization and deployment.
</p>

<p align="center">
 <img src="./logo.svg" alt="Ashveil Logo" width="220" />
</p>

<p align="center">
 <img src="https://img.shields.io/badge/Build-Static%20Web-success" alt="Static Web" />
</p>

---

## Overview

Ashveil is a small static loading-screen project styled around the visual identity of Fallout: New Vegas and the Mojave.

It is intended for Garry's Mod server loading URLs, but it can also be hosted as a normal static webpage.

The project has no build system and no backend.

## Features

- Fallout-inspired dark and orange interface
- Animated radar-style loading graphic
- Rotating server hints
- Smooth hint fade transitions
- Responsive layout
- Static deployment
- GitHub Pages compatibility
- Easy text and theme customization
- No server-side runtime required

## Quick Start

Clone the repository:

```bash
git clone https://github.com/bleonheart/Ashveil.git
cd Ashveil
```

Start a local static server:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Garry's Mod Usage

After hosting the page publicly, use the hosted URL as your server loading-screen URL.

For GitHub Pages:

```text
https://bleonheart.github.io/Ashveil/
```

The project is static, so any public host capable of serving HTML and CSS can be used.

## Customization

### Server Hints

Hints are defined in the `hints` array inside `index.html`.

```javascript
var hints = [
  "First server hint",
  "Second server hint",
  "Third server hint"
];
```

The page cycles through each message automatically.

### Hint Interval

The current interval is controlled by:

```javascript
setInterval(cycleHints, 3000);
```

The value is measured in milliseconds.

### Visual Theme

Most presentation styling is contained in `style.css`.

This includes:

- Background styling
- Accent colors
- Radar animation
- Borders
- Typography
- Layout and spacing
- Loading-screen presentation

## External Browser Resources

The current page loads a small number of browser resources from CDNs, including:

- Google Fonts
- Normalize.css
- jQuery

An internet connection is therefore required for those externally hosted resources unless they are replaced with local copies.

## Repository Structure

```text
Ashveil/
├── index.html
├── style.css
└── README.md
```

## Hosting

Ashveil can be deployed through:

- GitHub Pages
- Nginx
- Apache
- Static web hosts
- Garry's Mod loading-screen hosting
- Local HTTP servers for testing

## Contributing

Improvements to the layout, responsiveness, animations, accessibility, customization, or loading-screen integration are welcome.

1. Fork the repository
2. Create a feature branch
3. Make and test your changes
4. Open a pull request describing the improvement

---

<p align="center">
 <strong>A simple Mojave-themed loading experience with no build pipeline.</strong>
</p>

---

## License

This project is licensed under the [PolyForm Noncommercial License 1.0.0](https://polyformproject.org/licenses/noncommercial/1.0.0).

Use, modification, and redistribution are permitted only for purposes allowed by that license. Commercial use is not licensed under these terms.

See [LICENSE](./LICENSE) for details.
