# js-linting

1.Configure eslint: `npx eslint --init`

```bash 
✔ How would you like to use ESLint? · style
✔ What type of modules does your project use? · commonjs
✔ Which framework does your project use? · none
✔ Does your project use TypeScript? · No / Yes
✔ Where does your code run? · browser
✔ How would you like to define a style for your project? · guide
✔ Which style guide do you want to follow? · airbnb
✔ What format do you want your config file to be in? · JSON
```

2. Install plugin: `https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint`
3. Configure prettier: `npm i --save-dev prettier eslint-config-prettier eslint-plugin-prettier`
4. After installing these three packages, open your .eslintrc.json file in VSCode and add in the “extends” section the string “prettier”. Like this:

```json
"extends": [
  "airbnb-base",
  "prettier"
],
```
Then create the key “plugins” and add “prettier” to the array. Like this:

```json
"extends": [
  "airbnb-base",
  "prettier"
],
"plugins": [
  "prettier"
]
```
The last change is to add a new rule in the “rules” key, like this:

```json
"rules": {
  "prettier/prettier": "error"
}
```

5. Autocorrect in vscode
`mkdir .vscode` and `touch .vscode/settings.json` --> 
```json
{
  "editor.formatOnSave": true
}
```

6. Add prettier config 
`touch prettier.config.js && touch .prettierignore`

```javascript
  module.exports = {
    tabWidth: 2,
    semi: true,
    singleQuote: false,
    trailingComma: "es5",
  };
```
