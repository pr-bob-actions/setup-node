# Setup Node action for Github Action

This action use [actions/setup-node](https://github.com/actions/setup-node) and:

- activate yarn with corepack (useful for self-hosted runners)
- enable cache for yarn

## Input

All inputs refer to [actions/setup-node](https://github.com/actions/setup-node)'s inputs

- `node-version`: Specify the version of Node (default: `lts`)
- `cache`: Specify the package manager used (default: `yarn`)
- `cache-dependency-path`: Specifiy the lock file for cache reference (default: `**/yarn.lock`)

## How to use

```yaml
- uses: pr-bob-actions/setup-node@v1
  with:
    node-version: 16
```
