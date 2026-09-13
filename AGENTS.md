## Development

Start the dev server with background mode:

```
astro dev --background
```

Manage it with `astro dev stop`, `astro dev status`, and `astro dev logs`.

## Verification

No lint, typecheck, or test scripts are configured. The built-in check is a production build:

```
npm run build
```

`astro check` is not set up — it would prompt to install `@astrojs/check` and `typescript`, which are not in this repo.

## Stack

- Plain Astro 7.x, requires Node >= 22.12.0 (see `engines` in `package.json`). `astro` is the only dependency: no framework integrations, content collections, or Tailwind.
- Build output goes to `dist/`. `.astro/` (generated types) is created on dev/build and is gitignored.

## Documentation

https://docs.astro.build