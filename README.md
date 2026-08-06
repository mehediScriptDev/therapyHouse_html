# 🏋️ Athletic Alignment Lab — Frontend Web Application

Welcome to the **Athletic Alignment Lab** frontend repository! This is a modern, high-performance, fast-loading static website designed for Athletic Alignment Lab — a premier athletic alignment, pain recovery, and body performance lab.

This codebase is built using **clean, semantic HTML5**, **modular Vanilla CSS3**, and **lightweight ES6+ JavaScript**, eliminating heavy framework overhead to deliver maximum performance, fast load times, and superior SEO.

---

## 📑 Table of Contents

- [✨ Project Overview](#-project-overview)
- [🚀 Key Features](#-key-features)
- [🛠️ Tech Stack](#️-tech-stack)
- [📂 Project Directory Structure](#-project-directory-structure)
- [⚡ Quick Start & Local Development](#-quick-start--local-development)
- [🏗️ Architectural Guidelines](#️-architectural-guidelines)
- [🤝 How to Contribute](#-how-to-contribute)
- [🖼️ Image Optimization Guide](#️-image-optimization-guide)
- [🌐 Deployment](#-deployment)
- [📞 Support & Contact](#-support--contact)

---

## ✨ Project Overview

**Athletic Alignment Lab** provides targeted body alignment, mobility restoration, and pain relief for athletes and active individuals.

This repository houses the entire customer-facing frontend interface, which includes:

- **Home Page (`index.html`)**: Hero section, service highlights, process walkthrough, social proof, and FAQ accordion.
- **Packages & Services (`packages.html`)**: Comprehensive package pricing, session details, and booking calls to action.
- **About Us (`about.html`)**: Brand mission, philosophy, and team details.
- **Partnerships (`partnerships.html`)**: Affiliate and business collaboration opportunities.
- **Contact (`contact.html`)**: Direct inquiry form, location, and contact information.

---

## 🚀 Key Features

- 📱 **Fully Responsive Layout**: Built mobile-first using CSS Flexbox and Grid.
- ⚡ **Zero-Framework Speed**: Instant page loads with standard web APIs.
- 🎨 **Modern Design System**: CSS Custom Properties (Variables) for consistent colors, typography, spacing, and smooth dark/light design touches.
- ✨ **Scroll Animations**: Smooth entrance animations powered by `IntersectionObserver`.
- ❓ **Interactive FAQ Accordion**: Expandable FAQ items with smooth CSS transitions.
- 🍔 **Mobile Drawer Navigation**: Custom slide-out navigation overlay with keyboard accessibility (`Escape` key support) and click-outside closing.
- 🖼️ **Next-Gen Image Formats**: Assets converted to lightweight `.webp` format for minimal bandwidth usage.

---

## 🛠️ Tech Stack

- **Markup**: HTML5 (Semantic & Accessible)
- **Styling**: Vanilla CSS3 (Variables, Flexbox, Grid, Animations)
- **Scripting**: ES6+ JavaScript (Modular scripts, DOM Manipulation, Web APIs)
- **Icons**: FontAwesome 6 (CDN-based SVG icons)
- **Fonts**: Google Fonts (Inter & custom typography)
- **Image Processing**: Node.js + `sharp` library for image compression

---

## 📂 Project Directory Structure

```text
yusef_atx_frontend/
├── 📄 index.html          # Main landing page
├── 📄 about.html          # About page
├── 📄 packages.html       # Packages & pricing page
├── 📄 partnerships.html   # Partnerships & affiliate page
├── 📄 contact.html        # Contact & inquiry page
│
├── 📁 css/                # Stylesheets directory
│   ├── 🎨 style.css       # Global styles, typography, header, footer, & reusable utility components
│   ├── 🎨 index.css       # Home page specific styles
│   ├── 🎨 about.css       # About page specific styles
│   ├── 🎨 packages.css    # Packages page specific styles
│   ├── 🎨 partnerships.css# Partnerships page specific styles
│   └── 🎨 contact.css     # Contact page specific styles
│
├── 📁 js/                 # JavaScript scripts directory
│   ├── 📜 script.js       # Main global JS (Sticky Header, Mobile Nav, Scroll Reveal, FAQ Accordions)
│   ├── 📜 index.js        # Home page specific JS logic
│   ├── 📜 about.js        # About page specific JS logic
│   ├── 📜 packages.js     # Packages page specific JS logic
│   ├── 📜 partnerships.js # Partnerships page specific JS logic
│   └── 📜 contact.js      # Contact page specific JS logic
│
├── 📁 img/                # WebP images & brand graphic assets
├── 📄 package.json        # Project metadata & npm dependencies (e.g. sharp)
└── 📄 README.md           # Project documentation
```

---

## ⚡ Quick Start & Local Development

Because this project is a pure static web app, no build step or complex server setup is strictly required to run it!

### Option 1: VS Code Live Server (Recommended)

1. Install the **Live Server** extension in Visual Studio Code.
2. Right-click [`index.html`](file:///c:/dev/yusef_atx_frontend/index.html) and select **Open with Live Server**.
3. Browser will automatically launch at `http://127.0.0.1:5500`.

### Option 2: Node `npx serve`

If you have Node.js installed:

```bash
# Run local dev server from the project root
npx serve .
```

### Option 3: Python HTTP Server

```bash
# Python 3
python -m http.server 8000
```

Open `http://localhost:8000` in your browser.

---

## 🏗️ Architectural Guidelines

To maintain code clarity and consistency, future developers should follow these conventions:

### 1. HTML Conventions

- Use semantic HTML tags (`<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`, `<article>`).
- Always include `alt` tags on `<img>` elements for accessibility.
- Maintain unique `id` attributes for key interactive elements.

### 2. CSS Conventions

- **Global Tokens**: Always check [`css/style.css`](file:///c:/dev/yusef_atx_frontend/css/style.css) for CSS variable definitions (`:root` colors, font sizes, spacing, header height).
- **Page Specific Styles**: Put page-specific layout code inside the corresponding file (e.g., [`css/contact.css`](file:///c:/dev/yusef_atx_frontend/css/contact.css)).
- **Class Naming**: Follow clear BEM-like or descriptive standard class names (e.g. `.faq-item`, `.faq-question`, `.nav-link`).

### 3. JavaScript Conventions

- Wrap script logic inside IIFEs `(function() { "use strict"; ... })();` or use modules to avoid polluting the global window scope.
- Always check if an element exists before adding event listeners (`if (myEl) { ... }`).
- Use passive event listeners for performance-sensitive scroll events.

---

## 🤝 How to Contribute

We welcome contributions! Follow these easy steps to get started:

### Step 1: Clone or Fork the Repository

```bash
git clone <repository-url>
cd yusef_atx_frontend
```

### Step 2: Create a Feature Branch

Create a branch named after the feature or fix you are working on:

```bash
git checkout -b feature/add-new-section
# or for bug fixes:
git checkout -b fix/mobile-nav-bug
```

### Step 3: Make Your Changes

- Edit the corresponding HTML file, CSS file in `css/`, or JS file in `js/`.
- Ensure changes are responsive across mobile (375px+), tablet (768px+), and desktop (1024px+).

### Step 4: Test Locally

- Verify layout integrity across Chrome, Firefox, and Safari mobile views.
- Open Developer Tools Console to ensure **zero JavaScript errors**.

### Step 5: Commit & Push

```bash
git add .
git commit -m "feat: add new testimonial section to index.html"
git push origin feature/add-new-section
```

### Step 6: Create a Pull Request (PR)

Submit a Pull Request with a short title and description explaining what was added or changed.

---

## 🖼️ Image Optimization Guide

All website imagery should be optimized to `.webp` format to ensure sub-second page loads.

Dependencies are pre-configured in `package.json` with `sharp`. If you need to convert heavy `.jpg` or `.png` images:

1. Install dependencies:
   ```bash
   npm install
   ```
2. Convert and resize images using Node scripts or command-line sharp utilities before placing output files inside the `img/` folder.

---

## 🌐 Deployment

This static site can be deployed instantly to any web server or static host:

- **Vercel / Netlify**: Simply link your GitHub repository. Root directory is `/`, build command is blank, output directory is `.`.
- **GitHub Pages**: Go to Repository Settings -> Pages -> Source: `main` branch.
- **Traditional Web Server (Nginx / Apache)**: Copy all files to your web document root (e.g. `/var/www/html`).

---

## 📞 Support & Contact

For questions or assistance regarding this repository:

- 📩 Email: `meheduvau@gmail.com`
- 🌐 Website: Athletic Alignment Lab

_Happy coding! 🚀_
