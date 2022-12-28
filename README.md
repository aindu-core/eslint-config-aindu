👮‍♂️ Aindu ESLint + Prettier configuration
===
Opinionated linting configuration based on [eslint-config-codely](https://github.com/CodelyTV/eslint-config-codely), with some extra checks.

# Use and config:
You only need to extend your eslint config (`.eslintrc.js`) with this config, for that your first need to install the dependency:

```sh
npm install --save-dev eslint-config-aindu
```

## For JavaScript
```js
{
  extends: [ "eslint-config-aindu" ]
}
```
## For TypeScript
```js
{
  extends: [ "eslint-config-aindu/typescript" ],
  overrides: [
    {
      files: ["*.ts", "*.tsx"],
      parserOptions: {
        project: ["./tsconfig.json"],
      },
    },
  ]
}
```