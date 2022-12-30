# Dorayaki ESLint Config

[ESlint](https://eslint.org/) config used for Dorayaki.js.

## Usage

Do you want to add the config to your own projects? There you go:

1. Add this package to your devDependencies

```bash
$ npm i -D @dorayakijs/eslint-config
# or
$ yarn add -D @dorayakijs/eslint-config
```

2. Install `eslint` if not already present locally or globally

```bash
$ npm i -D eslint
# or
$ yarn add -D eslint
```

3. Create a `.eslintrc` file

4. Extend our config (you can use just the scope name as ESLint will assume the `eslint-config` prefix):

```json
{
  "extends": [
    "@dorayakijs"
  ]
}
```

## Full example

A full example `.eslintrc` for a project with babel support:
> Dont forget to `npm i -D babel-eslint` or `yarn add -D babel-eslint`

```json
{
  "root": true,
  "parserOptions": {
    "parser": "babel-eslint",
    "sourceType": "module"
  },
  "extends": [
    "@dorayakijs"
  ]
}
```

## TypeScript

If you're using TypeScript, follow [Usage](#usage) section by replacing `@dorayakijs/eslint-config` by `@dorayakijs/eslint-config-typescript`.

And in your `.eslintrc` all you need is :

```json
{
  "extends": [
    "@dorayakijs/eslint-config-typescript"
  ]
}
```

You can then edit/override same rules as you could with `@dorayakijs/eslint-config` but also TypeScript rules.
You can find the list of supported TypeScript rules [here](https://github.com/typescript-eslint/typescript-eslint/tree/master/packages/eslint-plugin#supported-rules).

## License

Setup inspired by [eslint-config-standard](https://github.com/standard/eslint-config-standard)

MIT - Dorayaki.js team
