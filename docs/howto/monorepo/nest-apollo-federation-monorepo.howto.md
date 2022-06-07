# Nest monorepo & graphql federation packages

## Generate apps & libs

### Setup project

```
 nest new facthub-gateway
```

### Setup apps

```
cd facthub-gateway
```

```
nest generate app facthub-user
```

```
nest generate app facthub-customer
```

```
nest generate app facthub-product
```

```
nest generate app facthub-order
```

```
nest generate app facthub-transporter
```

```
nest generate app facthub-warehouse
```

### Setup Libraries

```
nest generate library facthub-repository
```

```
nest generate library facthub-entity
```

```
nest generate library facthub-resolver
```

```
nest generate library facthub-service
```

---

## Install graphql packages

```
pnpm add @nestjs/graphql @nestjs/apollo graphql apollo-server-express
```

```
pnpm add @apollo/federation @apollo/gateway
```

```
pnpm add @apollo/subgraph
```

---

## Running the app

- Services :

```
pnpm start facthub-customer-application
```

```
pnpm start facthub-order-application
```

```
pnpm start facthub-product-application
```

- Gateway : services should be deployed.

```bash
$ pnpm start
```
