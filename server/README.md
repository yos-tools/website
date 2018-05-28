# yos.server
The **yos.tools** server is a kickstarter for your API services.

It provides the preconfigured core, useful services and help functions as well as basic APIs, so that the **yos.server** itself can be extended as a complete API server or used as a "[kernel](https://en.wikipedia.org/wiki/Kernel_(operating_system))" in the form of an integrated npm package in your project.

All provided APIs and services can be configured or completely overwritten so that the core can be flexibly integrated into any project and adapted to the required conditions.

With the help of [hooks](https://en.wikipedia.org/wiki/Hooking) it is possible to change objects and data in the various processes if necessary.

Our goal is to create a simple and flexible basis with which an API server can be set up very quickly so that the developers can concentrate on the business logic of the respective project.

# Technolgies
It's based on following technologies:
- [Node.js](https://nodejs.org) to run [JavaScript](https://en.wikipedia.org/wiki/JavaScript) on server
- [npm](https://www.npmjs.com) to manage JavaScript packages

In the future, the server will support all common APIs: [GraphQL](https://graphql.org), [REST](https://en.wikipedia.org/wiki/Representational_state_transfer), ... We start with the implementation of GraphQL via [Apollo Server](https://www.apollographql.com/server) integrated in [Express](http://expressjs.com).

Due to the implementation in different architecture layers it is not only possible to use different API types simultaneously, but also to realize a flexible connection of different [SQL](https://en.wikipedia.org/wiki/SQL) and [NoSQL](https://en.wikipedia.org/wiki/NoSQL) databases such as [MySQL](https://www.mysql.com/) and [MongoDB](https://www.mongodb.com/what-is-mongodb). First, we focus on MongoDB via [Typegoose](https://github.com/szokodiakos/typegoose), building on [mongoose](http://mongoosejs.com).

For the implementation we work with [Typescript](https://www.typescriptlang.org/) to use JavaScript in a structured and [type-safe](https://en.wikipedia.org/wiki/Type_safety) way. You do not necessarily have to work with Typescript to implement your API, you can also use [Coffescript](https://coffeescript.org) or pure JavaScript ([Vanilla JS](http://vanilla-js.com/)).

# Preparations
Before starting, check that you have installed the following software
- [Node.js](https://nodejs.org) and [npm](https://www.npmjs.com) via the node version managers [n](https://github.com/mklement0/n-install) ([n-install](https://github.com/mklement0/n-install)) or [nvm](https://github.com/creationix/nvm)
- [VuePress](https://vuepress.vuejs.org/guide/getting-started.html) (if you want to use it as documentation generator)