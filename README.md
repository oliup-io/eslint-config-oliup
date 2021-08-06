# Oliup Coding Guidelines for JAVASCRIPT

We use [eslint](https://eslint.org/) for linting (and prettier for formatting, depends on your editor)

## Setting up

Install eslint

```bash
npm install -g eslint # globally
# or
npm install --save-dev eslint # locally
```

Install oliup config

```bash
npm install --save-dev  github:oliup-io/eslint-config-oliup
```

## Web Project

This section is for any javascript code that will run in a web browser.

```bash
cd /path/to/your/project
touch .eslintrc.json
```

In the `.eslintrc.json` file created above copy & save the following config

```json
{
  "env": {
    "node": false,
    "browser": true
  },
  "parserOptions": {
    "ecmaVersion": 5
  },
  "extends": "eslint-config-oliup",
  "rules": {}
}
```

## NodeJS

This section is for server side javascript code.

```bash
cd /path/to/your/project
touch .eslintrc.json
```

In the `.eslintrc.json` file created above copy & save the following config

```json
{
  "env": {
    "node": true,
    "browser": false,
    "commonjs": true,
    "es2021": true
  },
  "extends": "eslint-config-oliup",
  "rules": {}
}
```
