# oapi-doc

ThingsPro OAPI document

# OAPI URL

- [ThingsPro Server](https://thingspro-server-oapi.netlify.com)
- [ThingsPro Gateway](https://thingspro-gateway-oapi.netlify.com)
- [ThingsPro Edge](https://thingspro-edge-oapi.netlify.com)

# Development

## Dependencies

- node >= v8
- yarn

## Setup

```sh
yarn
```

## Add New Swagger Document

```sh
# name must be gateway, server or edge
mkdir -p packages/oapi-tp-<name>/schema/<name>
touch packages/oapi-tp-<name>/schema/index.yaml
```

Note: after create document, remember to add reference in packages/oapi-tp-gateway/schema/index.yaml

## Validation

```sh
yarn lint <name> # name must be gateway, server or edge
```

## Preview

```sh
yarn build <name> && yarn start <name> # name must be gateway, server or edge
```
