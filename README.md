# shopify store front Monorepo

This repository contains the source code for **shopify store front** – a collection
of Shopify-specific commerce components, hooks and utilities that can be used
across multiple React frameworks (Next.js, Gatsby, etc.) to build headless
custom storefronts.

The monorepo is structured using a [turbo](https://turbo.build/) workspace. It
hosts multiple packages and apps:

- `packages/react` – the main library published as `@shopify/shopify-store-front`.
  See [packages/react/README.md](packages/react/README.md) for detailed
  documentation, installation instructions and development guides.
- `apps/nextjs` – an example Next.js application built with shopify store front.

## Getting started

1. **Clone the repository**

   ```bash
   git clone https://github.com/Shopify/shopify-store-front.git
   cd shopify-store-front
   ```

2. **Install dependencies**

   ```bash
   npm install
   # or `yarn install` if you prefer yarn
   ```

3. **Run the example app**

   ```bash
   cd apps/nextjs
   npm run dev
   ```

   The example should be available at `http://localhost:3000`.


## Packages

This monorepo currently exposes:

- `@shopify/shopify-store-front` – the core library containing components, hooks,
  types and utilities that interact with Shopify storefronts.

Additional packages may live here in the future; refer to the `packages/`
directory for a complete list.

## Documentation

- **Official docs**: https://shopify.dev/docs/api/shopify-store-front
- **Overview guide**: https://shopify.dev/custom-storefronts/shopify-store-front
- **Package-specific README**: [packages/react/README.md](packages/react/README.md)

## Development

Development scripts are managed through the workspace root. Some common
commands include:

```bash
# run linting across all packages
npm run lint

# run tests in the react package
npm --workspace packages/react run test

# build all packages
npm run build
```

The `apps/nextjs` directory contains a sample project; you can also run
`npm --workspace apps/nextjs run dev` to start that app in development mode.

## Contributing

We welcome contributions! Please review [CONTRIBUTING.md](CONTRIBUTING.md) for
guidelines around issues, pull requests, and code style.

Some pointers:

- Ensure new features or bug fixes include appropriate tests.
- Update changelogs located in `packages/*/CHANGELOG.md` using the `changeset`
  workflow.
- Follow the existing TypeScript and React patterns used throughout the codebase.

Questions or help? Join the Discord community: https://discord.gg/Hefq6w5c5d

---

<p align="center">📦 Built with ❤ by Shopify</p>
