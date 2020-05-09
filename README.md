# sapper-template

The default [Sapper](https://github.com/sveltejs/sapper) template, available for Rollup and webpack.


## Getting started


### Using `degit`

[`degit`](https://github.com/Rich-Harris/degit) is a scaffolding tool that lets you create a directory from a branch in a repository. Use either the `rollup` or `webpack` branch in `sapper-template`:

```bash
# for Rollup
npx degit "sveltejs/sapper-template#rollup" my-app
# for webpack
npx degit "sveltejs/sapper-template#webpack" my-app
```


### Running the project

However you get the code, you can install dependencies and run the project in development mode with:

```bash
cd my-app
npm install # or yarn
npm run dev
```

Open up [localhost:3000](http://localhost:3000) and start clicking around.

Consult [sapper.svelte.dev](https://sapper.svelte.dev) for help getting started.


## Set up environment variables

1. Create a `.env` file:

```bash
NEWSLETTER_API_TOKEN=XXX
```

2. Include it in `.gitignore` so you don't commit it accidentally

3. Install `dotenv` package

```bash
yarn add dotenv
```

4. Bootstrap `dotenv` in `drc/server.js` file

5. Add `NEWSLETTER_API_TOKEN` in session by using `sapper.middleware`

6. You can check how you can access `NEWSLETTER_API_TOKEN` in `preload` function of `src/routes/index.svelte` page component

7. You can check how you can access `NEWSLETTER_API_TOKEN` through `session` store across every component in `src/components/Nav.svelte` component
