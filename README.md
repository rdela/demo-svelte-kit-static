# demo-svelte-kit-static

This ultra-simple static Svelte Kit example is on GitHub at [rdela/demo-svelte-kit-static](https://github.com/rdela/demo-svelte-kit-static) and deployed to Netlify at [svelte-static.netlify.app](https://svelte-static.netlify.app/).

[Watch Rich Harris’ talk on YouTube](https://www.youtube.com/watch?v=qSfdtmcZ4d0) for background and other examples of this brand new, still experimental way to build [Svelte](https://svelte.dev/) apps that reimagines [Sapper](https://sapper.svelte.dev/) with [Snowpack](https://www.snowpack.dev/) baked in. Imagine [Create Snowpack App’s Svelte Template](https://www.snowpack.dev/#create-snowpack-app-(csa)) with all of Sapper’s abilities plus serverless superpowers.

## create-svelte

Everything you need to build a Svelte project, powered by [`create-svelte`](https://github.com/sveltejs/kit/tree/master/packages/create-svelte);

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npm init svelte@next

# create a new project in my-app
npm init svelte@next my-app
```

> Note: the `@next` is temporary

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

Svelte apps are built with *adapters*, which optimise your project for deployment to different environments, like [Begin](https://begin.com), [Netlify](https://www.netlify.com), [Vercel](https://vercel.com) and so on. (You can also create your own adapter — instructions TODO.)

By default, `npm run build` uses `adapter-node` to generate a Node app that you can run with `node build`. Here we are using `adapter-static` to create a static site, the equivalent of `sapper export`. To use a different adapter, install it and update your `svelte.config.js` accordingly. The following official adapters are available:

* [@sveltejs/adapter-node](https://github.com/sveltejs/kit/tree/master/packages/adapter-node)
* [@sveltejs/adapter-static](https://github.com/sveltejs/kit/tree/master/packages/adapter-static)
* [@sveltejs/adapter-netlify](https://github.com/sveltejs/kit/tree/master/packages/adapter-netlify)
* ...more soon
