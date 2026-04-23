# Dev Container Setup

This project includes a development container configuration that provides a consistent development environment with all necessary tools and extensions pre-configured.

## What's Included

### Development Tools
- **Node.js LTS** - For running the development server
- **npm** - Package management and scripts
- **serve** - Lightweight development server (runs on port 5000)

### VS Code Extensions
- **HTML/CSS Support** - Enhanced HTML and CSS editing
- **CSS IntelliSense** - Autocomplete for CSS properties and values
- **Tailwind CSS IntelliSense** - Even though not using Tailwind, provides great CSS utilities
- **Prettier** - Code formatting
- **Live Server** - Quick preview server (port 5500)
- **ESLint** - JavaScript linting
- **GitLens** - Enhanced Git capabilities
- **Markdown Preview** - Preview markdown files
- **Auto Rename Tag** - Automatically rename paired HTML tags
- **Path IntelliSense** - Autocomplete for file paths

### VS Code Settings
- Format on save enabled
- Prettier as default formatter
- Emmet enabled for HTML
- CSS validation enabled
- HTML validation enabled

## Getting Started

1. **Open in Dev Container**
   - Use Command Palette: `Dev Containers: Reopen in Container`
   - Or click the "Reopen in Container" button when prompted

2. **Dependencies are automatically installed** via `postCreateCommand`

3. **Start Development Server**
   - Run Task: `Tasks: Run Task > Start Dev Server`
   - Or use terminal: `npm run dev`
   - Open http://localhost:5000 in your browser

## Available Tasks

- **Start Dev Server** - Launches the portfolio on port 5000
- **Install Dependencies** - Reinstall npm packages
- **Format Code** - Format HTML, CSS, JSON, and Markdown files

## Ports

- **5000** - Main development server (serve)
- **5500** - Live Server preview (alternative)

## Development Workflow

1. Make changes to `index.html` or `styles.css`
2. Save files (auto-formatting will apply)
3. View changes at http://localhost:5000
4. Use Live Server for quick static previews if needed

## Customization

The dev container configuration can be customized by editing:
- `.devcontainer/devcontainer.json` - Container setup and extensions
- `.devcontainer/tasks.json` - Available development tasks

## Troubleshooting

- If extensions don't install, try reloading the window
- If ports aren't forwarding, check the Ports panel in VS Code
- For dependency issues, run `Tasks: Run Task > Install Dependencies`