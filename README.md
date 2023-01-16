👮‍♂️ Aindu ESLint + Prettier configuration
===
<p align="center">
    <img src="https://avatars.githubusercontent.com/u/121467350?s=400&u=c2cd1b3deea96ddb8dae7cec440d50791907202f&v=4" width="300px" height="180px"
/>
</p>

Opinionated linting configuration based on [eslint-config-codely](https://github.com/CodelyTV/eslint-config-codely), with some extra checks.

# Use and config:
You only need to extend your eslint config (`.eslintrc.js`) with this config, for that your first need to install the dependency:

```sh
npm install --save-dev eslint-config-aindu
```

## For JavaScript
```js
module.exports = {
  extends: [ "eslint-config-aindu" ]
}
```
## For TypeScript
```js
module.exports = {
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