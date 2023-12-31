# Roadiz Nuxt 3 Minimal Starter and Layer

## Migration from Nuxt2 starter TODO list

- [x] Roadiz API plugin `$apiFetch` and global *useAsyncData*
- [x] Parse and render apiFetch hydra-error
- [x] Block factory
- [x] Page SEO
- [x] InterventionRequest nuxt-image provider
- [x] Sitemap from Roadiz nodes-sources
- [x] `VForm` and form elements factory from JSON schema
- [x] Preview aware routing with `_preview` query parameter and JWT bearer \
    Using `usePreview` state composable and global route middleware
- [x] Bug: Same i18n locale in server and client at first request \
    Need to set locale again in `app:beforeMount` hook
- [ ] Bug: `ArticleContainer` component is instantiated twice on SSR
- [ ] Bug: i18n locale messages are not loaded on production build
- [ ] SVG loader
- [x] Storybook integration
- [ ] Themeable and ThemeProvider composables
- [ ] HTTP cache middleware
- [x] eslint configuration
- [ ] CI/CD configuration
- [ ] Docker configuration
- [x] SCSS configuration
- [ ] Basic components

## Examples

Theses blocks components are available:

- Basic block: `components/blocks/BasicBlock.vue`
- Group block: `components/blocks/GroupBlock.vue`

## Override Nuxt runtime configuration

You can override Nuxt runtime configuration by creating a `.env` file at the root of your project and
using `NUXT_PUBLIC` prefix on any **existing** config vars name.

```dotenv
# .env
NUXT_PUBLIC_BASE_URL=http://localhost:3000
NUXT_PUBLIC_API_BASE_URL=http://roadiz-core-app.test/api
NUXT_PUBLIC_INTERVENTION_REQUEST_BASE_URL=http://roadiz-core-app.test/assets
NUXT_PUBLIC_INTERVENTION_REQUEST_NO_PROCESS_BASE_URL=http://roadiz-core-app.test/images
``` 

---

Look at the [Nuxt 3 documentation](https://nuxt.com/docs/getting-started/introduction) to learn more.

## Setup

Make sure to install the dependencies:

```bash
# npm
npm install

# pnpm
pnpm install

# yarn
yarn install
```

## Development Server

Start the development server on `http://localhost:3000`:

```bash
# npm
npm run dev

# pnpm
pnpm run dev

# yarn
yarn dev
```

## Production

Build the application for production:

```bash
# npm
npm run build

# pnpm
pnpm run build

# yarn
yarn build
```

Locally preview production build:

```bash
# npm
npm run preview

# pnpm
pnpm run preview

# yarn
yarn preview
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.
