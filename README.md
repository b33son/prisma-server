Boilerplate for an Advanced GraphQL Server w/ TypeScript

Based on GraphQL boilerplate, typescript-advanced but uses Docker(https://blog.graph.cool/graphql-boilerplates-graphql-create-how-to-setup-a-graphql-project-6428be2f3a5).

## Requirements

You need to have the [GraphQL CLI](https://github.com/graphql-cli/graphql-cli) installed to bootstrap your GraphQL server using `graphql create`:

Globally install prisma and graphql-cli
npm i -g prisma
npm install -g graphql-cli

## Getting started

. Install via npm install
. Start your Prisma server: docker-compose up -d
. Deploy your Prisma service: prisma deploy
. Read more about Prisma server:
http://bit.ly/prisma-server-overview

## Documentation

### Commands

- `yarn start` starts GraphQL server on `http://localhost:4000`
- `yarn dev` starts GraphQL server on `http://localhost:4000` _and_ opens GraphQL Playground
- `yarn playground` opens the GraphQL Playground for the `projects` from [`.graphqlconfig.yml`](./.graphqlconfig.yml)
- `yarn prisma <subcommand>` gives access to local version of Prisma CLI (e.g. `yarn prisma deploy`)

## Features

- **Scalable GraphQL server:** The server uses [`graphql-yoga`](https://github.com/prisma/graphql-yoga) which is based on Apollo Server & Express
- **Static type generation**: TypeScript types for GraphQL queries & mutations are generated in a build step
- **Authentication**: Signup and login workflows are ready to use for your users
- **GraphQL database:** Includes GraphQL database binding to [Prisma](https://www.prismagraphql.com) (running on MySQL)
- **Tooling**: Out-of-the-box support for [GraphQL Playground](https://github.com/prisma/graphql-playground) & [query performance tracing](https://github.com/apollographql/apollo-tracing)
- **Extensible**: Simple and flexible [data model](./database/datamodel.graphql) – easy to adjust and extend
- **No configuration overhead**: Preconfigured [`graphql-config`](https://github.com/prisma/graphql-config) setup
- **Realtime updates**: Support for GraphQL subscriptions
