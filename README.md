# NextJS ESM Example 2021

An example that uses [ESM](https://github.com/standard-things/esm#readme) with
[Next.js](https://nextjs.org/) and yarn workspaces.

Based on https://github.com/curran/nextjs-esm-example but stripping the Lerna
dependency in favor of Yarn workspaces and assuming modern versions of Node (>12).

The idea behind this is to show a simple working example of how you can define
multiple packages for a single project, and import ES6 modules from your
packages (rather than be restricted to CommonJS import and export).

## Usage

- Run `yarn install` or just `yarn` in the root
- `cd packages/nextjs-with-express/`
- `yarn dev` to start the dev server
- Then access http://localhost:3000/

The page should display "Importing an ES6 module in Next.js via ESM worked!".
This is interesting because it's imported directly as an ES6 module from within
`node_modules` (sym-linked by Yarn Workspaces).

## More Information

- [Next.js Custom Server with Express
  example](https://github.com/zeit/next.js/blob/canary/examples/custom-server-express).
- [A practical guide to
  ESM](https://gist.github.com/sindresorhus/a39789f98801d908bbc7ff3ecc99d99c)
