# A Svelte + Rollup + PostCSS + Tailwind CSS starter

This is a starter for a Web UI project that uses:
- the lovely [Svelte](https://svelte.dev/) JS framework
- with the efficient [rollup.js](https://rollupjs.org/) module bundler
- and [PostCSS](https://postcss.org/) tool for optimizing the CSS result
- and the absolutely gorgeous [Tailwind CSS](https://tailwindcss.com/) framework

All the instructions below consider [pnpm](https://pnpm.js.org/) tool, instead of the classic NPM, again, just from an efficient point of view.

<br/>

## Setup

`pnpm i` to install the dependencies.

## Running in Dev mode

Run _in development mode_ using `pnpm run dev` or the included `run_dev.sh` script.

Navigate to [localhost:5000](http://localhost:5000) to access the app.

<br/>

## Building and Running in Production mode

Use `pnpm run build` to create an optimised version of the app, ready to be deployed.

Use `pnpm run start` to  run the newly built app.

<br/>

## Single-page app (SPA) mode

By default, sirv will only respond to requests that match files in `public`. This is to maximise compatibility with static fileservers, allowing you to deploy your app anywhere.

If you're building a single-page app (SPA) with multiple routes, sirv needs to be able to respond to requests for *any* path. You can make it so by editing the `"start"` command in package.json:

```js
"start": "sirv public --single"
```
