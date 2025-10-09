# nextgenit-site

A modern, futuristic Vue 3 + Vite landing page for NextGenIT meetups, designed for deployment on Cloudflare Pages.

## Features

- 🚀 Built with Vue 3 and Vite for fast development and optimized production builds
- 📱 Fully responsive design with mobile-first approach
- 🎨 Dark theme with NextGenIT brand colors (#00FFD1, #FE005B, #18204E)
- ✨ Animated particle background with floating elements
- 🔮 Glassmorphism effects with neon glow animations
- 🎯 Interactive logo with hover effects and shimmer animation
- 📱 Social media links with animated hover states
- 🌟 Smooth animations and transitions throughout
- ♿ Accessibility-friendly with proper semantic HTML and focus states
- 🔍 SEO optimized with meta tags and Open Graph support
- ⚡ Static site generation for optimal performance
- 🎭 Modern typography with Alatsi font from Google Fonts

## Development

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Deployment

The project is configured for Cloudflare Pages deployment:

1. Build command: `npm run build`
2. Output directory: `dist`

The production-ready static files are generated in the `/dist` directory after running the build command.

## Project Structure

```
nextgenit-site/
├── src/
│   ├── App.vue      # Main application component
│   ├── main.js      # Vue app entry point
│   └── main.css     # Global styles with modern CSS
├── index.html       # HTML entry point
├── vite.config.js   # Vite configuration
└── package.json     # Dependencies and scripts
```

## Technologies

- **Vue 3**: Progressive JavaScript framework with Composition API
- **Vite**: Next-generation frontend tooling with fast HMR
- **Modern CSS**: Custom properties, glassmorphism, animations, and responsive design
- **Google Fonts**: Alatsi font for modern typography
- **CSS Animations**: Keyframe animations and transitions
- **Glassmorphism**: Backdrop filters and translucent elements
- **Neon Effects**: Box shadows and glow effects for futuristic look

## License

MIT License - see [LICENSE](LICENSE) file for details