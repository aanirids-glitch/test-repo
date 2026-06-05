# Tech Stack & Libraries

## Core Technologies

| Category | Technology | Purpose |
|----------|------------|---------|
| **Runtime** | Node.js (LTS) | JavaScript runtime environment |
| **Framework** | React 18+ | Component-based UI library |
| **Build Tool** | Vite | Fast build tool and dev server |
| **Language** | JavaScript (ES2020+) | Primary programming language |
| **Package Manager** | npm / Yarn | Dependency management |

## Development Dependencies

### Build & Bundling
- `@vitejs/plugin-react` - Vite plugin for React (uses Oxc)
- `@vitejs/plugin-react-swc` - Alternative SWC-based plugin

### Code Quality
- `eslint` - JavaScript linting utility
- `@eslint/js` - ESLint core configuration
- `eslint-plugin-react` - React specific linting rules
- `eslint-plugin-react-hooks` - Rules for React Hooks

### Testing (Recommended)
- `vitest` - Fast unit test runner
- `@testing-library/react` - React component testing utilities
- `jest-dom` - Custom Jest matchers for DOM testing

### Type Safety (Recommended)
- `typescript` - Typed superset of JavaScript
- `@typescript-eslint/eslint-plugin` - TypeScript ESLint plugin
- `@typescript-eslint/parser` - TypeScript parser for ESLint

## Optional Additions

### Routing
- `react-router-dom` - Declarative routing for React

### State Management
- `zustand` - Small, fast state management
- `@reduxjs/toolkit` - Redux toolkit for complex state
- `react-context` - Built-in context API

### Styling
- `tailwindcss` - Utility-first CSS framework
- `styled-components` - CSS-in-JS styling
- `sass` / `less` - CSS preprocessors

### Backend Integration
- `axios` / `fetch` - HTTP client
- `react-query` / `swr` - Data fetching and caching

### Utilities
- `lodash-es` - Utility library
- `date-fns` - Date utility functions

## Project Structure Recommendations

```
src/
├── components/     # Reusable UI components
├── hooks/          # Custom React hooks
├── pages/          # Page-level components
├── services/       # API and external service integrations
├── store/          # State management (if using Redux/Zustand)
├── utils/          # Helper functions
├── assets/         # Images, fonts, static files
├── App.jsx         # Main application component
└── main.jsx        # Application entry point
```

## Environment Variables

Create a `.env` file in the root directory:

```env
VITE_API_URL=http://localhost:3000/api
VITE_APP_TITLE=Test Repo
```

**Note:** Vite requires `VITE_` prefix for variables to be exposed to the client.