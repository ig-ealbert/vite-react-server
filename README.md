# Vite React Server

## Overview

I wanted to make a project template for React with a server.  I had worked with [`create-react-app`](https://create-react-app.dev/) in the past but it is now deprecated.

I would also like it to be in TypeScript, but when I tried this using `vite-extra`, it said that `"ssr-react-ts" isn't a valid template`, even though it is listed on their [website](https://github.com/bluwy/create-vite-extra/tree/master?tab=readme-ov-file#scaffolding-your-first-vite-project).

I'm also surprised that the generated code does not use semicolons.  That's recommended.

```
npm create vite-extra@latest vite-react-server -- --template ssr-react
```

## Changes I Made

1. Installed TypeScript and various types packages.
2. Added `.tsconfig.json` and `.tsconfig.node.json`.
3. Changed `.jsx` files to `.tsx`.
4. Updated `server.js` to have imports at the top.

I wasn't able to update the `server.js` to `server.ts` as it `Cannot find module` when I do that.

## How to Run

```
npm install
npm run build
npm run preview
```

## Links

* [Vite Extra](https://github.com/bluwy/create-vite-extra/tree/master?tab=readme-ov-file#scaffolding-your-first-vite-project)
* [Vite.js Getting Started](https://vitejs.dev/guide/#scaffolding-your-first-vite-project)
* [React TypeScript Template Without Server](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts)
* [Create React App (deprecated)](https://create-react-app.dev/docs/getting-started)