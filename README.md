# Angular SSR Application

This is a basic Angular application with Server-Side Rendering (SSR) support.

## Prerequisites

- Node.js (v18 or higher)
- npm (comes with Node.js)

## Setup

1. Install dependencies:
```bash
npm install
```

## Development

### Client-Side Development Server
Run the standard Angular development server:
```bash
npm start
```
Navigate to `http://localhost:4200/`

### SSR Development Server
Run the application with Server-Side Rendering:
```bash
npm run dev:ssr
```
Navigate to `http://localhost:4200/`

## Build

### Standard Build (Client-Side Only)
```bash
npm run build
```

### SSR Build
Build the application with SSR support:
```bash
npm run build:ssr
```

### Serve SSR Build
After building with SSR, serve the application:
```bash
npm run serve:ssr:angular-app
```
The app will be available at `http://localhost:4000/`

## Prerendering

Generate static pages at build time:
```bash
npm run prerender
```

## Project Structure

```
angular-app/
├── src/
│   ├── app/
│   │   ├── app.component.ts       # Root component
│   │   ├── app.component.html     # Root template
│   │   ├── app.component.css      # Root styles
│   │   ├── app.config.ts          # Application configuration
│   │   ├── app.config.server.ts   # Server configuration
│   │   └── app.routes.ts          # Route definitions
│   ├── assets/                    # Static assets
│   ├── index.html                 # Main HTML file
│   ├── main.ts                    # Client entry point
│   ├── main.server.ts             # Server entry point
│   └── styles.css                 # Global styles
├── server.ts                      # Express server for SSR
├── angular.json                   # Angular CLI configuration
├── package.json                   # Project dependencies
└── tsconfig.json                  # TypeScript configuration
```

## What is SSR?

Server-Side Rendering (SSR) renders your Angular application on the server before sending it to the browser. This provides:

- **Better SEO**: Search engines can crawl your content more effectively
- **Faster Initial Load**: Users see content faster on slow connections
- **Improved Performance**: Especially on low-powered devices

## Learn More

- [Angular Documentation](https://angular.dev)
- [Angular SSR Guide](https://angular.dev/guide/ssr)
- [Angular CLI](https://angular.dev/cli)

## License

MIT


