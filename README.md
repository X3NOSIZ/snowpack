[![CI](https://github.com/pikapkg/snowpack/workflows/CI/badge.svg?event=push)](https://github.com/pikapkg/snowpack/actions)

### What is Snowpack?

**Snowpack is a modern, lightweight toolchain for web application development.** Traditional dev bundlers like webpack or Parcel need to rebuild & rebundle entire chunks of your application every time you save a single file. This introduces lag between changing a file and seeing those changes reflected in the browser, sometimes as slow as several seconds.

Snowpack solves this problem by serving your application **unbundled in development.** Any time you change a file, Snowpack never rebuilds more than a single file. There's no bundling to speak of, just a few milliseconds of single-file rebuilding and then an instant update in the browser via HMR. We call this new approach **O(1) Build Tooling.** You can read more about it in our [Snowpack 2.0 Release Post.](https://www.snowpack.dev/posts/2020-05-26-snowpack-2-0-release/)

When you're ready to deploy your web application to users, you can add back a traditional bundler like Webpack or Parcel. With Snowpack you get bundled & optimized production performance without sacrificing dev speed by adding an unnecessary bundler,

### Key Features

- A dev environment that starts up in **50ms or less.**
- Changes are reflected [instantly in the browser.](https://www.snowpack.dev/posts/2020-05-26-snowpack-2-0-release/#hot-module-replacement)
- Integrates your favorite bundler for [production-optimized builds.](https://www.snowpack.dev/posts/2020-05-26-snowpack-2-0-release/#snowpack-build)
- Out-of-the-box support for [TypeScript, JSX, CSS Modules and more.](https://www.snowpack.dev/posts/2020-05-26-snowpack-2-0-release/#features)
- Connect your favorite tools with [third-party plugins.](https://www.snowpack.dev/posts/2020-05-26-snowpack-2-0-release/#build-plugins)

**💁 More info at the official [Snowpack website ➞](https://snowpack.dev)**

## Create Snowpack App (CSA)

For starter apps and templates, see [create-snowpack-app](./packages/create-snowpack-app).

## Official Snowpack Plugins

### Dev Environment

- [@snowpack/plugin-dotenv](./packages/plugin-dotenv)

### Build

- [@snowpack/plugin-babel](./packages/plugin-babel)
- [@snowpack/plugin-svelte](./packages/plugin-svelte)
- [@snowpack/plugin-vue](./packages/plugin-vue)

### Transform

- [@snowpack/plugin-postcss](./packages/plugin-postcss)
- [@snowpack/plugin-react-refresh](./packages/plugin-react-refresh)

### Bundle

- [@snowpack/plugin-parcel](./packages/plugin-parcel)
- [@snowpack/plugin-webpack](./packages/plugin-webpack)

### Advanced Plugins

- [@snowpack/plugin-build-script](./packages/plugin-build-script)
- [@snowpack/plugin-run-script](./packages/plugin-run-script)

### Featured Community Plugins

- [@prefresh/snowpack](https://github.com/JoviDeCroock/prefresh)
- [snowpack-plugin-import-map](https://github.com/zhoukekestar/snowpack-plugin-import-map) A more easy way to map your imports to Pika CDN instead of [import-maps.json](https://github.com/WICG/import-maps).
- PRs that add a link to this list are welcome!
