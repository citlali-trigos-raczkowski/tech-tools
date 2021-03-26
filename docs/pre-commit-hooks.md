# Husky and Lint-staged - pre-commit hook managers

- [Husky](https://typicode.github.io/husky/#/)
- [Lint-staged](https://www.npmjs.com/package/lint-staged)

### Installation

```
npm install prettier husky lint-staged es-lint
```

### Sample `package.json`:

```
    "eslintConfig"" {
        "parser": "@typescript-eslint/parser",
        "rules": {
            "no-unused-vars": "off",
            ...
        }

    },
    "prettier"" {
        "singleQuote": true,
        "arrowParens": "avoid"
    }
    "husky": {
        "hooks": {
            "pre-commit": "lint-staged"
        },
    },
    "lint-staged": {
        "src/**/*.{js,jsx,ts,tsx,json,css}": [
            "prettier --write",
            "eslint --fix ",
            "npm test"
        ]
    }

```
