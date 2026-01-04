# Template Repository

A modern JavaScript development template with Webpack, Babel, ESLint, and Prettier pre-configured.

## Features

- 🔧 **Webpack 5** - Module bundling with dev/prod configurations
- 🎯 **Babel** - Modern JavaScript transpilation
- ✨ **ESLint** - Code linting
- 💅 **Prettier** - Code formatting
- 🪝 **Husky** - Git hooks for code quality
- 📦 **Split configs** - Separate dev and production builds

## Prerequisites

- Node.js 20+ (see `.nvmrc`)
- npm or yarn

## Getting Started

1. **Use this template:**
   Click "Use this template" button on GitHub

2. **Install dependencies:**

```bash
   npm install
```

3. **Start development:**

```bash
   npm run dev
```

4. **Build for production:**

```bash
   npm run build
```

## Available Scripts

- `npm run dev` - Start development server with hot reload
- `npm run build` - Build for production
- `npm run lint` - Run ESLint
- `npm run format` - Format code with Prettier
- `npm run format:check` - Check code formatting

## Project Structure

```
├── src/              # Source files
├── dist/             # Production build (generated)
├── .husky/           # Git hooks
├── webpack.common.js # Shared Webpack config
├── webpack.dev.js    # Development config
├── webpack.prod.js   # Production config
└── package.json
```

## Browser Support

Modern browsers (> 0.25% market share, not dead)
