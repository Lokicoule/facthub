# Nest monorepo & graphql federation packages

## Generate apps & libs

```bash
$ nest new facthub-gateway
$ cd facthub-gateway
$ nest generate app facthub-user-application
$ nest generate app facthub-customer-application
$ nest generate app facthub-product-application
$ nest generate app facthub-order-application
$ nest generate app facthub-transporter-application
$ nest generate app facthub-warehouse-application

$ nest generate library facthub-core-lib
$ nest generate library facthub-auth-lib
```

---

## Install graphql packages

```bash
$ pnpm add @nestjs/graphql @nestjs/apollo graphql apollo-server-express

$ pnpm add @apollo/federation @apollo/gateway

$ pnpm add @apollo/subgraph
```

---

## Running the app

- Services :

```bash
$ npm start facthub-customer-application
$ npm start facthub-order-application
$ npm start facthub-product-application
```

- Gateway : services should be deployed.

```bash
$ npm start
```
