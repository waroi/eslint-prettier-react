# eslint-prettier-react

## Installation

```bash
npm i -D eslint-prettier-react
```

### or with yarn

```bash
yarn add -D eslint-prettier-react
```
### you need to install the following packages

```bash
yarn add --dev eslint-plugin-react
```

## Usage

Create a file named `.eslintrc.js` in the root of your project and add the following:

```js
module.exports = {
  extends: ['eslint-prettier-react'],
};
```

add a file named `.prettierrc` in the root of your project and add the following:

```json
{
    "semi": true,
    "singleQuote": true,
    "tabWidth": 2,
    "trailingComma": "es5",
    "printWidth": 100,
    "arrowParens": "always",
    "importOrder": [
        "^components/(.*)$",
        "^[./]"
    ],
    "importOrderSeparation": false,
    "importOrderSortSpecifiers": true
}
```

package.json

```json
{
  "scripts": {
    "lint": "eslint . --ext .js,.jsx,.ts,.tsx",
    "lint:fix": "eslint . --ext .js,.jsx,.ts,.tsx --fix",
    "format": "prettier --write .",
    "format:check": "prettier --check ."
  }
}
```

## Temp Rules

```js
rules: {
    // TODO: test maçlı kapama
    "react/prop-types": ["off"],
    "no-unused-vars": ["off"],
    "no-use-before-define": ["off"],
    "no-shadow": ["off"],
    "import/extensions": ["off"],
    "no-console": ["off"],
    "no-unsafe-optional-chaining": ["off"],
    "radix": ["off"],
    "no-nested-ternary": ["off"],
    "react/jsx-no-useless-fragment": ["off"],
    "camelcase": ["off"],
    "import/no-named-as-default": ["off"],
    "react/no-unescaped-entities": ["off"],
    "eqeqeq": ["off"],
    "react/no-array-index-key": ["off"],
    "no-undef": ["off"],
    "react/no-unused-prop-types": ["off"],
    "react/no-unknown-property": ["off"],
    "react/default-props-match-prop-types": ["off"],
    "react/destructuring-assignment": ["off"],
    "react/no-unstable-nested-components": ["off"],
    "no-await-in-loop": ["off"],
    "react/jsx-no-constructed-context-values": ["off"],
    "no-constant-condition": ["off"],
    "no-alert": ["off"],
    "import/no-extraneous-dependencies": ["off"],
    "no-inner-declarations": ["off"],
    "no-return-await": ["off"],
    "react-hooks/exhaustive-deps": ["off"],
    "array-callback-return": ["off"],
    "no-async-promise-executor": ["off"],
    "func-names": ["off"],
    "no-restricted-globals": ["off"],
    "no-irregular-whitespace": ["off"],
    "no-empty": ["off"],
    "no-sequences": ["off"],
    "no-eval": ["off"], // Güvenlik açığı oluşturabilir.
    "import/no-named-as-default-member": ["off"],
    "no-prototype-builtins": ["off"],
    "prefer-destructuring": ["off"],
    "no-lone-blocks": ["off"],
    "no-useless-escape": ["off"],
    "react/no-danger": ["off"], // Güvenlik açığı oluşturabilir.
    "import/no-unresolved": ["off"],
    "jsx-a11y/no-noninteractive-element-interactions": ["off"],
    "no-restricted-syntax": ["off"],
    "no-loop-func": ["off"],
    "react/no-this-in-sfc": ["off"],
    "default-param-last": ["off"],
    "no-lonely-if": ["off"],
    "import/no-duplicates": ["off"],
    "operator-assignment": ["off"],
    "prefer-const": ["off"],
    "no-cond-assign": ["off"],
    "no-case-declarations": ["off"],
    "default-case": ["off"],
    "react/jsx-no-undef": ["off"],
    "react-hooks/rules-of-hooks": ["off"],
    "no-duplicate-case": ["off"],
    "no-bitwise": ["off"],
    "react/no-typos": ["off"],
    // Todo: test maçlı kapama
}
```
