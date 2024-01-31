# @shawnphoffman/prettier-config

Prettier shared config for all of my projects.

## Usage

1. Remove existing `.prettierrc` or other [Prettier config files](https://prettier.io/docs/en/configuration.html) if present.
1. Create (or add to) an `.npmrc` file the following content:
   ```
   @shawnphoffman:registry=https://npm.pkg.github.com
   ```
1. Install directly from GitHub:

   ```
   yarn add -D @shawnphoffman/prettier-config
   ```

1. Add the following to `package.json`:

   ```
   "prettier": "@shawnphoffman/prettier-config"
   ```

## Development

1. Edit rules in [prettier.config.js](prettier.config.js).
1. Bump version number in [package.json](package.json).
1. Push.
1. The [npm-publish-github-packages.yml](.github/workflows/npm-publish-github-packages.yml) workflow will automatically publish a new version.
