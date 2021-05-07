# demo-svelte-kit-static

This ultra-simple static Svelte Kit example is on GitHub at [rdela/demo-svelte-kit-static](https://github.com/rdela/demo-svelte-kit-static) and deployed to Netlify at [svelte-static.netlify.app](https://svelte-static.netlify.app/).

## Create your own from scratch

```bash
npm init svelte@next my-app

cd my-app

npm install

npm run dev -- --open
```

More complete instructions below and in the docs.

## Learn more

Visit [kit.svelte.dev](https://kit.svelte.dev) to read the SvelteKit documentation.

For background on this new, still experimental way to build [Svelte](https://svelte.dev/) apps that reimagines [Sapper](https://sapper.svelte.dev/), you can watch Rich Harris’ talks on YouTube [An update on SvelteKit](https://www.youtube.com/watch?v=fnr9XWvjJHw&t=19102s)  from Apr 25, 2021, or the precursor, [Futuristic Web Development](https://www.youtube.com/watch?v=qSfdtmcZ4d0) from Oct 19, 2020. Or you can read the blog posts:

- [What's new in Svelte: May 2021 - New in SvelteKit](https://svelte.dev/blog/whats-new-in-svelte-may-2021#New_in_SvelteKit)
- [SvelteKit is in public beta](https://svelte.dev/blog/sveltekit-beta)
- Introductory post: [What's the deal with SvelteKit?](https://svelte.dev/blog/whats-the-deal-with-sveltekit)

## create-svelte

Everything you need to build a Svelte project, powered by [`create-svelte`](https://github.com/sveltejs/kit/tree/master/packages/create-svelte);

### Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npm init svelte@next

# create a new project in my-app
npm init svelte@next my-app
```

> Note: the `@next` is temporary

### Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

### Building

Before creating a production version of your app, install an [adapter](https://kit.svelte.dev/docs#adapters) for your target environment. Then:

```bash
npm run build
```

> You can preview the built app with `npm run preview`, regardless of whether you installed an adapter. This should _not_ be used to serve your app in production.
