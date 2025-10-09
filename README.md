# nextgenit-site

A minimal, responsive Vue 3 + Vite landing page for NextGenIT, designed for deployment on Cloudflare Pages.

## Features

- 🚀 Built with Vue 3 and Vite for fast development and optimized production builds
- 📱 Fully responsive design with mobile-first approach
- 🎨 Modern gradient background with smooth animations
- ♿ Accessibility-friendly with proper semantic HTML and focus states
- 🎯 Centered logo placeholder and clean typography
- 🔮 Prepared structure for animated backgrounds and social icons
- ⚡ Static site generation for optimal performance

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

- **Vue 3**: Progressive JavaScript framework
- **Vite**: Next-generation frontend tooling
- **Modern CSS**: Custom properties, gradients, and responsive design

## License

MIT License - see [LICENSE](LICENSE) file for details