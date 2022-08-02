# Wincket Subgraph

TheGraph exposes a GraphQL endpoint to query the events and entities within the Binance Smart Chain.

Currently, there are multiple subgraphs, but additional subgraphs can be added to this repository, following the current architecture.

## Dependencies

- [Graph CLI](https://github.com/graphprotocol/graph-cli)
    - Required to generate and build local GraphQL dependencies.

```shell
yarn global add @graphprotocol/graph-cli
```

## Deployment

1. Run the `cd subgraphs/wincket` command to move to the subgraph directory.

2. Run the `yarn codegen` command to prepare the TypeScript sources for the GraphQL (generated/*).

3. Run the `yarn build` command to build the subgraph, and check compilation errors before deploying.

4. Run `graph auth --product hosted-service '<ACCESS_TOKEN>'`

5. Deploy via `yarn deploy`.
