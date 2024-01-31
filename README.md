# prettier-config

Prettier shared config for all RouteIf projects.

## Usage

Usage is based on [Sharing configurations](https://prettier.io/docs/en/configuration.html#sharing-configurations) from the Prettier docs. The package is [retrieved from GitHub Packages](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-npm-registry#installing-a-package).

1. Remove existing `.prettierrc` or other [Prettier config files](https://prettier.io/docs/en/configuration.html) if present.
1. Create (or add to) an `.npmrc` file the following content:
    ```
    @routeif:registry=https://npm.pkg.github.com
    ```
1. Install directly from GitHub:

    ```
    npm install -D @routeif/prettier-config
    OR
    pnpm add -D @routeif/prettier-config
    ```

1. Add the following to `package.json`:

    ```
    "prettier": "@routeif/prettier-config"
    ```

## Development

1. Edit rules in [prettier.config.js](prettier.config.js).
1. Bump version number in [package.json](package.json).
1. Push.
1. The [push.yml](.github/workflows/push.yml) workflow will automatically publish a new version.
