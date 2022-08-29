---
tags: Fronends, Eslint
---

## Step 1: Install
```bash=
yarn add -D eslint
yarn add -D eslint-plugin-react eslint-plugin-css-modules eslint-config-airbnb eslint-plugin-import eslint-plugin-react-hooks eslint-plugin-jsx-a11y @typescript-eslint/eslint-plugin @typescript-eslint/parser

# init eslint configration
./node_modules/.bin/eslint --init
```

Choose the option by the following steps:
1. To check syntax, find problems, and enforce code style
2. JavaScript modules (import/export)
3. None of these (react/ vue)
4. Yes for typescript.
5. Browser (if for frontend) - (node for backend).
6. Use a popular style guide: `airbnb`
7. JavaScript -- format for eslint config
8. Would you like to install them now with npm? › `No` -> if you use `yarn`

## Step 2: Config Eslint
- Install Eslint extension + Prettier in VSCode
- Open setting (JSON) of VS code: add configs to this file `setting.json`
```json = 
// should use another combined key to format
"editor.codeActionsOnSave": {
  "source.fixAll.eslint": false
},
"editor.formatOnSave": false,
"eslint.validate": ["javascript"],
```

## Step 3: Add rules:
Ref: https://eslint.org/docs/rules/
1. if you don't want to produce any error messages: `off` | `warn` | `error`
`"no-console": "off",`
2. Double quotes: 
`"quotes": ["error", "double"],`
3. Indent:
`"indent": ["error", 4],`

### Sample file: 
> I have attached 2 file config: `.eslintrc.js` and `.prettierrc` in this repository.
> Just copy both files to your project after installing eslint to `package.json`
# eslint-prettier-config
