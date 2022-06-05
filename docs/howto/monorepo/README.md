# Technical choice

## Nest monorepo

- pros
  - builtin
  - easy to add app
  - easy to add lib
- cons
  - one package.json
  - hard to configure for our needs
- Conclusion : easy to use but services are not purely isolated

## NX

- pros
- cons
  - one package.json
  - own cli
- Conclusion : services not isolated

## Turborepo

- pros
  - isolated apps with their own package.json
  - very configurable
- cons
  - little harder to configure
- Conclusion : best choice
