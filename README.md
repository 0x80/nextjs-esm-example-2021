# NextJS ESM Example 2021

A Next.js example that uses ES Modules and Yarn workspaces.

This was based on the example from https://github.com/curran/nextjs-esm-example
but strips the ESM and Lerna dependencies in favor of Yarn workspaces and modern
versions of Node with build-in ESM support.

The idea behind this is to show a simple working example of how you can define
multiple packages for a single project, and import ES6 modules from your
application (rather than be restricted to CommonJS import and export).

NPM also has workspaces nowadays, so I'm sure you can make it work with NPM
instead of yarn.

## Usage

### With Yarn

- Run `yarn install` or just `yarn` in the root
- `cd packages/nextjs-with-express/`
- `yarn dev` to start the dev server
- Then access http://localhost:3000/

### With NPM

@TODO try it out

The page should display "Importing an ES6 module in Next.js via ESM worked!".
This is interesting because it's imported directly as an ES6 module from within
`node_modules` (sym-linked by Yarn Workspaces).

## Some Useful Resources

- [Next.js Custom Server with Express
  example](https://github.com/zeit/next.js/blob/canary/examples/custom-server-express).
- [A practical guide to
  ESM](https://gist.github.com/sindresorhus/a39789f98801d908bbc7ff3ecc99d99c)
- [Yarn workspaces with Typescript](https://stackoverflow.com/questions/57679322/how-to-use-yarn-workspaces-with-typescript-and-out-folders)
