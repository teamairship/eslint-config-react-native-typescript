# Airship ESLint TypeScript React Native Config

[![npm package](https://img.shields.io/npm/v/@airship/eslint-config-react-native-typescript.svg?style=flat-square)](https://www.npmjs.org/package/@airship/eslint-config-react-native-typescript)

This is the shared [ESLint](https://eslint.org/) configuration file for [React Native](https://facebook.github.io/react-native/) [TypeScript](https://www.typescriptlang.org/) projects at [Airship](https://teamairship.com).

## Installation

```bash
yarn add -D typescript @airship/eslint-config-react-native-typescript
```

## Usage

In your ESLint config file, e.g. `.eslintrc`:

```javascript
{
  "parserOptions": {
    "project": "./tsconfig.json" // Don't forget to set this up :-)
  },
  "extends": ["@airship/eslint-config-react-native-typescript"]
}
```

If you need a starter `tsconfig.json` you can use this one:

```json
{
  "compilerOptions": {
    "allowJs": true,
    "allowSyntheticDefaultImports": true,
    "esModuleInterop": true,
    "isolatedModules": true,
    "jsx": "react-native",
    "lib": ["es6"],
    "module": "esnext",
    "moduleResolution": "node",
    "noEmit": true,
    "strict": true,
    "target": "esnext"
  },
  "exclude": [
    "node_modules",
    "babel.config.js",
    "metro.config.js",
    "jest.config.js"
  ]
}
```

## Contributing

Bug reports and pull requests are welcome on GitHub at [https://github.com/teamairship/tslint-react-config](https://github.com/teamairship/eslint-config-react-native-typescript). This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Code of Conduct](https://github.com/teamairship/eslint-config-react-native-typescript/blob/master/CODE_OF_CONDUCT.md).

## License

This package is available as open source under the terms of the [MIT License](https://github.com/teamairship/eslint-config-react-native-typescript/blob/master/LICENSE).
