# Technology Stack

This document provides a comprehensive overview of the technologies, programming languages, frameworks, and tools used in the Next.js project.

## Programming Languages

### JavaScript/TypeScript
- **TypeScript** (v5.9.2) - Primary language for type-safe JavaScript development
- **JavaScript** - Used throughout the codebase for Node.js and browser environments
- **Node.js** (v20+) - Runtime environment for server-side JavaScript execution

### Rust
- **Rust** - Used for high-performance native modules and compilation tools
  - SWC (Speedy Web Compiler) - Rust-based JavaScript/TypeScript compiler
  - Turbopack - Next-generation bundler written in Rust
  - Native bindings via NAPI for Node.js integration

## Core Framework & Libraries

### React Ecosystem
- **React** (v19.x) - Core UI library
- **React DOM** (v19.x) - DOM rendering for React
- **React Server Components** - Server-side rendering support
- **React Compiler** (experimental) - Optimization compiler for React

### Build Tools & Bundlers

#### Turbopack (Rust-based)
- **turbopack-core** - Core bundling functionality
- **turbopack-dev-server** - Development server
- **turbopack-ecmascript** - JavaScript/TypeScript processing
- **turbopack-css** - CSS processing
- **turbopack-node** - Node.js runtime support
- **turbopack-browser** - Browser runtime support
- **turbopack-wasm** - WebAssembly support
- **turbopack-mdx** - MDX file processing
- **turbopack-image** - Image optimization

#### Webpack (JavaScript-based)
- **Webpack** (v5.98.0) - Traditional JavaScript bundler
- **webpack-bundle-analyzer** - Bundle size analysis
- **webpack-dev-server** - Development server

#### Rspack (Alternative)
- **@rspack/core** (v1.6.7) - Rust-based Webpack-compatible bundler

### Compiler & Transpiler

#### SWC (Speedy Web Compiler)
- **@swc/core** (v1.11.24) - Rust-based JavaScript/TypeScript compiler
- **@swc/cli** - Command-line interface
- **@swc/helpers** - Runtime helpers
- **next-custom-transforms** - Custom Next.js transformations
- **swc_ecma_parser** - ECMAScript parser
- **swc_ecma_minifier** - Code minification

#### Babel
- **@babel/core** (v7.26.10) - JavaScript transpiler (legacy support)
- **@babel/parser** - JavaScript parser
- **@babel/generator** - Code generation
- **@babel/preset-react** - React transformation preset

## Monorepo & Package Management

### Workspace Management
- **pnpm** (v9.6.0) - Fast, disk-efficient package manager
- **Lerna** (v9.0.3) - Monorepo management tool
- **Turborepo** (v2.5.5) - High-performance build system

### Workspace Structure
- Multiple packages in `packages/` directory
- Rust crates in `crates/` directory
- Turbopack crates in `turbopack/crates/` directory

## Testing Frameworks

### Unit & Integration Testing
- **Jest** (v29.7.0) - JavaScript testing framework
- **@testing-library/react** - React component testing utilities
- **@testing-library/jest-dom** - Custom Jest matchers for DOM
- **jest-environment-jsdom** - Browser-like environment for tests
- **jest-extended** - Additional Jest matchers

### End-to-End Testing
- **Playwright** (v1.48.0) - Browser automation and E2E testing
- **playwright-chromium** - Chromium browser support

### Performance Testing
- **@vercel/devlow-bench** - Development and low-level benchmarking

## CSS & Styling

### CSS Processing
- **PostCSS** (v8.4.31) - CSS transformation tool
- **postcss-nested** - Nested CSS rules support
- **Tailwind CSS** (v3.2.7) - Utility-first CSS framework
- **Sass** (v1.54.0) - CSS preprocessor
- **lightningcss** - Fast CSS parser, transformer, and minifier
- **Critters** - Critical CSS extraction

### CSS-in-JS
- **styled-jsx** (v5.1.6) - CSS-in-JS library for Next.js
- **@emotion/react** - Emotion CSS-in-JS library
- **@emotion/cache** - Emotion caching

## Code Quality & Linting

### Linters
- **ESLint** (v9.37.0) - JavaScript/TypeScript linter
  - **eslint-plugin-react** - React-specific linting rules
  - **eslint-plugin-react-hooks** - React Hooks linting rules
  - **eslint-plugin-import** - Import/export linting
  - **eslint-plugin-jest** - Jest testing linting
  - **eslint-plugin-jsdoc** - JSDoc linting
  - **eslint-plugin-next** - Next.js-specific linting rules
- **@ast-grep/cli** - Structural code search and linting
- **alex** - Inclusive language linter
- **tsec** - TypeScript security linter

### Formatters
- **Prettier** (v3.6.2) - Code formatter
- **rustfmt** - Rust code formatter

### Type Checking
- **TypeScript** (v5.9.2) - Static type checking
- **@types/*** - TypeScript type definitions for various libraries

## Development Tools

### Task Runners
- **Taskr** - Task automation tool
- **npm-run-all** - Run multiple npm scripts in parallel

### Build Tools
- **Cargo** - Rust package manager and build tool
- **turbo** - Monorepo build orchestration
- **tsx** - TypeScript execution engine

### Version Control
- **Git** - Version control system
- **Husky** (v9.0.11) - Git hooks management
- **lint-staged** (v15.2.2) - Run linters on staged files

## Runtime & APIs

### Node.js Libraries
- **express** - Web application framework
- **cors** - CORS middleware
- **http-proxy** - HTTP proxying
- **cookie** - Cookie parsing and serialization
- **busboy** - Multipart form data parsing

### Edge Runtime
- **@edge-runtime/jest-environment** - Edge runtime testing environment

### OpenTelemetry
- **@opentelemetry/api** - Observability and tracing

## Data & Utilities

### Data Manipulation
- **lodash** - Utility library
- **moment** - Date/time manipulation
- **nanoid** - Unique ID generation
- **semver** - Semantic versioning

### File System
- **fs-extra** - Enhanced file system operations
- **glob** - File pattern matching
- **find-up** - Find files by walking up parent directories

### Process Management
- **cross-spawn** - Cross-platform process spawning
- **tree-kill** - Kill process trees
- **execa** - Process execution

## Third-Party Integrations

### Image Optimization
- **image-size** - Image dimension detection
- **is-animated** - Detect animated images
- **@vercel/og** - Open Graph image generation
- **satori** - SVG/HTML to image conversion

### Content Management
- **@mdx-js/loader** - MDX support for Webpack
- **@mdx-js/react** - MDX React integration
- **markdown** - Markdown parsing

### Fonts
- **@next/font** - Font optimization system

### Analytics & Monitoring
- **dd-trace** - Datadog APM tracing

## Cloud & Deployment

### Vercel Platform
- **@vercel/kv** - Vercel KV storage
- **Vercel deployment** - Optimized for Vercel platform

## Documentation Tools

- **Storybook** - Component documentation and development

## Additional Languages & Formats

### Configuration Languages
- **JSON** - Configuration and data files
- **YAML** - Configuration files
- **TOML** - Rust configuration (Cargo.toml)

### Markup Languages
- **Markdown** - Documentation and content
- **MDX** - Markdown with JSX components
- **HTML** - Web markup

### Styling Languages
- **CSS** - Cascading Style Sheets
- **SCSS/Sass** - CSS preprocessor
- **PostCSS** - CSS transformations

## WebAssembly (Wasm)

- **WebAssembly** - Low-level binary format for web
- **wasmer** - WebAssembly runtime
- **turbopack-wasm** - Wasm support in Turbopack

## Package Ecosystem

### Core Packages
- **next** - Main Next.js framework
- **create-next-app** - Next.js application scaffolding
- **@next/swc** - SWC integration
- **@next/mdx** - MDX integration
- **@next/env** - Environment variable handling
- **eslint-config-next** - ESLint configuration
- **eslint-plugin-next** - Next.js ESLint rules

## Security

- **tsec** - TypeScript security linter
- **CodeQL** - Security analysis (via GitHub Actions)
- **GitHub Security Advisories** - Vulnerability scanning

## Continuous Integration

- **GitHub Actions** - CI/CD pipeline
- **Turbo Remote Cache** - Build caching for CI

## License

Next.js is [MIT licensed](license.md).

---

**Note**: This technology stack is continuously evolving. For the most up-to-date information, refer to `package.json` and `Cargo.toml` in the repository.
