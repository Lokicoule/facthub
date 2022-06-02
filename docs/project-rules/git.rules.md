# Conventional Commits

## Commit type

| Type       |                                              Description |
| :--------- | -------------------------------------------------------: |
| `build`    |                  configuration and setup (npm, tsconfig) |
| `docs`     |            editing or updating documentation (README.md) |
| `feat`     |                                   feature implementation |
| `fix`      |                                                  bug fix |
| `refactor` | refactoring that doesn't affect the behavior of the code |
| `style`    |      doesn't bring any functional or semantic alteration |
| `test`     |                                      test implementation |
| `chore`    |                                             other change |

---

## Commit structural element

```
<type>(<*optional_scope>)<*optional_breaking_change>: <description>
```

- \*optional_breaking_change : !
- \*optional_scope : domain or file

### Examples

```
refactor(graphql)!: migrating to microservice using graphql-federation
```

Behavior doesn't change for api consumer but it's a breaking change because monolith application architecture migrated to microservice.

<details>
  <summary>References</summary>
  <p>

https://www.conventionalcommits.org/en/v1.0.0/

  </p>
</details>

---

## Control tool

https://commitlint.js.org/#/
