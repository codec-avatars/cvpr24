# CVPR 24 Workshop on Codec Avatars

## Before anything

Install nvm, the best way to get a recent npm:
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

Make sure you are using a recent version of npm, such as v20.10.0 aka `lts/iron`:

```bash
nvm install lts/iron
nvm use lts/iron
```

## Installing all deps

```bash
npm install
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.
