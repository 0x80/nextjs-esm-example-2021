# NextJS ESM JS/Typescript Example

An example of a modern Next.js project configuration.

This example uses Yarn workspaces because that is what I'm familiar withM, but NPM
also has workspaces nowadays and I would assume they are compatible.

## Javascript Only

For the stubborn who still like writing their code in plain Javascript, you can
check out the `topic/js-only` branch to see a working example before I've
converted it to Typescript.

## Features

- ES Modules
- Monorepo using Yarn or NPM workspaces
- Typescript with project references and incremental compilation
- Next.js 11 (including Webpack 5 and ESLint)

## Usage

### With Yarn

- Run `yarn install` or just `yarn` in the root
- `cd packages/nextjs-app/`
- `yarn dev` to start the dev server
- Then access http://localhost:3000/

The page should display "Importing an ES6 module in Next.js via ESM worked!".

### With NPM

@TODO try it out

### Future Improvements

- Figure out if it is possible to automatically build package dependencies when
  compiling the app.
- Add path alias for ~/

## Some Additional Resources

- [Next.js Custom Server with Express
  example](https://github.com/zeit/next.js/blob/canary/examples/custom-server-express).
- [A practical guide to
  ESM](https://gist.github.com/sindresorhus/a39789f98801d908bbc7ff3ecc99d99c)
- [Yarn workspaces with
  Typescript](https://stackoverflow.com/questions/57679322/how-to-use-yarn-workspaces-with-typescript-and-out-folders)
