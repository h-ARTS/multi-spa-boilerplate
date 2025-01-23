# Multi-SPA Boilerplate

A boilerplate repository for a multi-SPA (Single Page Application) monorepo setup with **Next.js**, including two separate Next.js applications.

## Features

-   **Multi-SPA Architecture**: Separate Next.js apps in one monorepo.
-   **Shared Code**: Easily share components, utilities, or configurations across apps.
-   **Optimized Development**: Supports fast builds and efficient development workflows.
-   **Extensible**: Add more SPAs or libraries as needed.

## Project Structure

```
multi-spa-boilerplate/
├── my-store/
│   ├── home/        # First Next.js application
│   │   ├── pages/
│   │   ├── public/
│   │   └── ...
│   ├── catalog/        # Second Next.js application
│   │   ├── pages/
│   │   ├── public/
│   │   └── ...
├── packages/           # Shared libraries or utilities (optional)
│   ├── ui/             # Example shared component library
│   └── utils/          # Example shared utilities
├── .gitignore
├── package.json
├── turbo.json          # Turborepo configuration (optional)
└── README.md
```

## Getting Started

1. **Clone the repository**:

    ```bash
    git clone https://github.com/your-username/multi-spa-boilerplate.git
    cd multi-spa-boilerplate
    ```

2. **Install dependencies**:

    ```bash
    npm install
    # or
    yarn install
    ```

3. **Run a development server**:
   Navigate to a specific app directory and start the server:

    ```bash
    cd apps/app-one
    npm run dev
    ```

    Or for the second app:

    ```bash
    cd apps/app-two
    npm run dev
    ```

    Access the apps at:

    - App One: `http://localhost:3000`
    - App Two: `http://localhost:3001` (if port configuration differs)

## Scripts

-   `dev`: Start development servers for apps.
-   `build`: Build the production versions of apps.
-   `lint`: Lint code for errors or style issues.
-   `test`: Run tests (if applicable).

## Shared Code

Use the `packages/` directory to store and share reusable code across the apps. Import shared components or utilities like:

```javascript
import { MySharedComponent } from '@myrepo/ui'
```

## Tools and Configurations

-   **Next.js**: Framework for both SPAs.
-   **Turborepo (optional)**: To manage builds and caching across apps.
-   **ESLint**: Linting and code style.
-   **TypeScript (optional)**: Type-safe development.

## Contributing

Feel free to open issues or submit pull requests to improve the boilerplate.

## License

[MIT](LICENSE)
