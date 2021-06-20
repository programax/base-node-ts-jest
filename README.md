# base-node-ts-jest

This is a template project to bootstrap a node app with typescript and jest. The idea is to setup the bare minimums for any project with typescript and save you the time to set it up from scratch. I tried not to make assumptions about the project structure or tech stack. That's the reason you will not find a single dependency (only dev dependencies). Do you need an express app? or appollo server? or something else? Go for it.

I made some assumptions about the project such as adding a Dockerfile, using eslint vs tslint, nodemon, yarn, opinionated paths config. However, all those things are very easy to remove. Seriously, it will take you 5 minutes to remove all of that.

# Inspiration

I found a bunch of templates on github for a node server with typescript, but they all had an opinionated project structure and tech stack. In addition, the npm scripts was polluted with way too many scripts that are probably never used. I wanted a simple project that I could clone with minimal assuptions about the toolset and no assumptions abou the tech stack and project structure. I feel like there are way too many node frameworks out there to start a new one, so that is not at all the idea of this template project. With that in mind I created this template to solve a sinlge purpose: provide a starting point for a typescript app with the bare minimums and make it easier to remove anything that is not needed.

# Getting started

If you look at the scripts in `package.json` you will figure out how this works in a few minutes. However, here is a summary:

### Dev

To start developing all you need is:

```bash
yarn install
yarn dev
```

That will start nodemon to watch for changes and make it easier to code without switching back and forth to the terminal.

### Test

I made the assumption of using jest so if you prefer something else I am sorry. Otherwise, all you need to do is:

```bash
yarn test
# OR
yarn test:watch
# OR
yarn test:coverage
```

You can probably figure out what they do by running them. I also added a nice jest plugin `jest-watch-typeahead` that allows you to autocomplete test names and file names, that makes it easier to focus on the test you care about.

### Lint

In case you have made huge changes and need to be sure typescript is not broken you can get all lint violations from ESLint and tsc like this:

```bash
# get linting for typescript compiler (tsc)
yarn type-check
# get linting for eslint
yarn lint
# or both
yarn check
```

### Build

If you want to make a build to get the js files and make a release you can do:

```bash
yarn build
yarn start
```

That is all, the compiled files will be found under `/build` ar the root. Running `yarn start` will start the app from the compiled files.
