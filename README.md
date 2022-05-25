# Next JS, GraphQL And Typescript

The code in this repository is based on the
[NextJS + GraphQL Blueprint: Professional Grade Setup](https://youtu.be/XzE-PzALyDc)
video.

Stopped the tutorial at 12 min 30 seconds.

Install graphql vscode plugin and create `.graphqlrc.json`.

Rename `pages/api/hello.js` to `*.ts` and when you run dev you will be
prompted to add typescript dependencies as note below.

```bash
yarn dev
yarn add --dev typescript @types/react @types/node
```

Add support for graphQl, apollo server and typeGraphQL.

```bash
yarn add graphql apollo-server-micro
yarn add micro
yarn add class-validator type-graphql reflect-metadata
# graph ql version has to be fixed to ^15.3.0 in package.json then
yarn install
# from the typegraphql.com site setup tsconfig.json
```

## GraphQL

```bash
curl --request POST \
  --header 'content-type: application/json' \
  --url http://localhost:3000/api/graphql \
  --data '{"query":"query getDogs { dogs { name } }"}'
```
