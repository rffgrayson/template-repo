# Template Repository

A modern JavaScript development template with Webpack, Babel, ESLint, and Prettier pre-configured.

## Features

- **Webpack 5** - Module bundling with dev/prod configurations
- **Babel** - Modern JavaScript transpilation
- **ESLint** - Code linting
- **Prettier** - Code formatting
- **Husky** - Git hooks for code quality
- **Split configs** - Separate dev and production builds
- **Bun support** - Fast alternative to npm (optional)
- **CI/CD** - GitHub Actions workflow included

## Prerequisites

**Choose one:**

- Node.js 20+ (see `.nvmrc`) with npm/yarn
- **OR** Bun 1.0+ (faster alternative)

## Getting Started

### 1. Use this template

Click the "Use this template" button on GitHub

### 2. Install dependencies

**Using npm (traditional):**

```bash
npm install
```

**Using Bun (faster):**

```bash
bun install
```

### 3. Start development

**With npm:**

```bash
npm run dev
```

**With Bun:**

```bash
bun run dev
```

### 4. Build for production

**With npm:**

```bash
npm run build
```

**With Bun:**

```bash
bun run build
```

## Available Scripts

| Command                                         | Description                              |
| ----------------------------------------------- | ---------------------------------------- |
| `npm run dev` / `bun run dev`                   | Start development server with hot reload |
| `npm run build` / `bun run build`               | Build optimized production bundle        |
| `npm run start` / `bun run start`               | Start dev server and open in browser     |
| `npm run lint` / `bun run lint`                 | Run ESLint on source files               |
| `npm run lint:fix` / `bun run lint:fix`         | Fix ESLint issues automatically          |
| `npm run format` / `bun run format`             | Format code with Prettier                |
| `npm run format:check` / `bun run format:check` | Check code formatting                    |
| `npm run deploy` / `bun run deploy`             | Deploy to GitHub Pages                   |

## Project Structure

```
template-repo/
├── .github/
│   └── workflows/
│       └── ci.yml        # GitHub Actions CI/CD
├── .husky/               # Git hooks configuration
├── src/                  # Source files
│   ├── index.js
│   └── ...
├── dist/                 # Production build (generated)
├── .babelrc              # Babel configuration
├── .editorconfig         # Editor configuration
├── .nvmrc                # Node.js version
├── bunfig.toml           # Bun configuration
├── eslint.config.js      # ESLint configuration
├── .prettierrc           # Prettier configuration
├── webpack.common.js     # Shared Webpack config
├── webpack.dev.js        # Development config
├── webpack.prod.js       # Production config
└── package.json          # Dependencies and scripts
```

## Browser Support

Modern browsers with > 0.25% market share (excludes dead browsers)

Configured via Babel's `@babel/preset-env` with automatic polyfill injection.

## CI/CD

This template includes a GitHub Actions workflow that automatically:

- ✅ Runs linting checks
- ✅ Verifies code formatting
- ✅ Tests production builds
- ✅ Tests with both npm and Bun

Workflow runs on every push and pull request to the `main` branch.

## Customization

### Change target browsers

Edit `.babelrc`:

```json
{
  "presets": [
    [
      "@babel/preset-env",
      {
        "targets": "> 0.5%, last 2 versions, not dead"
      }
    ]
  ]
}
```

### Modify linting rules

Edit `eslint.config.js`

### Adjust formatting

Edit `.prettierrc`

## Why This Template?

- ⚡ **Fast setup** - Start coding in minutes
- 🛠️ **Modern tooling** - Uses latest versions of build tools
- 🎯 **Best practices** - Pre-configured with industry standards
- 🔒 **Code quality** - Automated checks prevent bad commits
- 📦 **Flexible** - Works with npm or Bun

## License

MIT

---

**Happy coding!** If you find issues or have suggestions, please open an issue or PR.
