# StayBnB - Modern Vacation Rental Platform

A modern, responsive vacation rental website inspired by Airbnb's clean design philosophy and Apple's signature smooth animations. Built as a showcase of modern CSS techniques and best practices.

![StayBnB Preview](https://images.unsplash.com/photo-1501785888041-af3ef285b470?w=1200&h=600&fit=crop)

## Live Demo

**[View Live Site](https://pavankusunuri.github.io/hotels_flexbox/)**

The website is hosted on GitHub Pages and automatically deploys on every push to the `master` branch.

## About

StayBnB is a beautifully crafted vacation rental landing page that demonstrates:
- **Airbnb-inspired UI/UX**: Clean, minimalist design with intuitive navigation
- **Apple-style animations**: Smooth, spring-based transitions and scroll-triggered animations
- **Modern web standards**: Semantic HTML5, CSS Grid, Flexbox, and CSS Custom Properties

## Features

- **Responsive Design**: Fully optimized for desktop, tablet, and mobile devices
- **Smooth Animations**: 
  - Scroll-triggered fade-in animations
  - Spring-based hover effects
  - Parallax hero section with zoom animation
  - Staggered card animations
- **Interactive Elements**:
  - Category filter tabs
  - Favorite/heart button toggle
  - Header scroll effects
  - Hover state animations
- **Modern UI Components**:
  - Glassmorphism effects
  - Gradient text overlays
  - Custom SVG icons
  - Card-based property listings

## Tech Stack

| Technology | Purpose |
|------------|---------|
| **HTML5** | Semantic markup structure |
| **CSS3** | Styling with modern features |
| **CSS Grid** | Property listing grid layout |
| **Flexbox** | Component-level layouts |
| **CSS Custom Properties** | Theming and design tokens |
| **CSS Animations** | Keyframe animations and transitions |
| **SCSS/Sass** | CSS preprocessing (source files) |
| **JavaScript (Vanilla)** | Scroll animations and interactivity |
| **Google Fonts** | Inter font family |

## CSS Features Used

- **CSS Custom Properties (Variables)** - For consistent theming
- **CSS Grid** - For the property cards responsive grid
- **Flexbox** - For header, navigation, and component layouts
- **CSS Transforms & Transitions** - For smooth hover effects
- **CSS Animations** - For scroll-triggered and loading animations
- **Media Queries** - For responsive breakpoints
- **Backdrop Filter** - For glassmorphism effects
- **Clamp()** - For fluid typography

## Project Structure

```
hotels_flexbox/
├── index.html          # Main HTML file
├── css/
│   └── style.css       # Compiled CSS styles
├── sass/
│   ├── main.scss       # Main SCSS entry point
│   ├── _base.scss      # Base styles and variables
│   ├── _layout.scss    # Layout components
│   └── _components.scss # UI components
├── img/                # Image assets
│   └── SVG/            # SVG icons
├── .github/
│   └── workflows/
│       └── static.yml  # GitHub Pages deployment workflow
├── package.json        # Project dependencies
└── README.md           # This file
```

## Getting Started

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd hotels_flexbox
   ```

2. **Open in browser**
   Simply open `index.html` in your preferred browser

3. **For development with Sass** (optional)
   ```bash
   npm install
   npm run compile:sass
   ```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Design Inspiration

- **Airbnb** - Clean, trust-building UI with focus on imagery
- **Apple** - Smooth, spring-based animations and scroll effects
- **Modern SaaS** - Card-based layouts and glassmorphism

## Key Design Decisions

1. **Color Palette**: Coral/pink primary color (#FF385C) matching Airbnb's brand identity
2. **Typography**: Inter font for clean, modern readability
3. **Animations**: Cubic-bezier curves for Apple-like spring animations
4. **Layout**: CSS Grid for responsive property cards, Flexbox for everything else
5. **Spacing**: Consistent spacing scale using CSS custom properties

## Performance Optimizations

- Intersection Observer for scroll animations (only animate visible elements)
- CSS transforms instead of layout-triggering properties
- Optimized image URLs with width/height parameters
- Minimal JavaScript footprint

## Deployment

This project is automatically deployed to **GitHub Pages** using GitHub Actions.

### How It Works

1. **GitHub Actions Workflow**: A workflow file (`.github/workflows/static.yml`) is configured to trigger on every push to the `master` branch

2. **Automatic Deployment**: When code is pushed:
   - GitHub Actions checks out the repository
   - Uploads the static files as an artifact
   - Deploys to GitHub Pages

3. **Live URL**: The site is served at `https://pavankusunuri.github.io/hotels_flexbox/`

### Workflow Configuration

```yaml
# Triggers on push to master branch
on:
  push:
    branches: ["master"]

# Deploys using GitHub's official Pages actions
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/configure-pages@v5
      - uses: actions/upload-pages-artifact@v3
      - uses: actions/deploy-pages@v4
```

### Setting Up GitHub Pages

To enable GitHub Pages for your own fork:

1. Go to **Settings** > **Pages** in your repository
2. Under **Source**, select **GitHub Actions**
3. Push to `master` branch to trigger deployment

## License

This project is open source and available for learning purposes.

---

**Built with modern web technologies | Hosted on GitHub Pages**
