# base-node-ts-jest

This is a template project to bootstrap a node app with typescript and jest. The idea is to setup the bare minimums for any project with typescript and save you the time to set it up from scratch. I tried not to make assumptions about the project structure or tech stack. That's the reason you will not find a single dependency (only dev dependencies). Do you need an express app? or appollo server? or something else? Go for it.

I made some assumptions about the project such as adding a Dockerfile, using eslint vs tslint, nodemon, yarn, opinionated paths config. However, all those things are very easy to remove. Seriously, it will take you 5 minutes to remove all of that.

# Inspiration

I found a bunch of templates on github for a node server with typescript, but they all had an opinionated project structure and tech stack. In addition, the npm scripts was polluted with way too many scripts that are probably never used. I wanted a simple project that I could clone with minimal assuptions about the toolset and no assumptions abou the tech stack and project structure. I feel like there are way too many node frameworks out there to start a new one, so that is not at all the idea of this template project. With that in mind I created this template to solve a sinlge purpose: provide a starting point for a typescript app with the bare minimums and make it easier to remove anything that is not needed.
