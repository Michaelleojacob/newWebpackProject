## npm init -y

## npm install webpack webpack-cli --save-dev

## npm install --save-dev css-loader

## npm install style-loader --save

## npm install html-loader style-loader --save

## npm install eslint --save-dev

## npm i --save-dev html-webpack-plugin

## `or one liner:`

## npm install webpack webpack-cli css-loader html-loader eslint dotenv-webpack html-webpack-plugin --save-dev

## mkdir src dist

## touch src/index.html src/script.js package.json webpack.config.js .env

# ./node_modules/.bin/eslint --init

### ? How would you like to use ESLint? …

- To check syntax only
- To check syntax and find problems
- `❯ To check syntax, find problems, and enforce code style`

### ? What type of modules does your project use? …

- JavaScript modules (import/export)
- `❯ CommonJS (require/exports)`
- None of these

### ? Which framework does your project use? …

- React
- Vue.js
- `❯ None of these`

### ? Does your project use TypeScript? › No / Yes`

- `❯ No`
- yes

### ? Where does your code run?`

- `❯ Browser`
- Node

### ? ✔ How would you like to define a style for your project? …

- `❯ Use a popular style guide`
- Answer questions about your style
- Inspect your JavaScript file(s)

### ? What format do you want your config file to be in? …

- JavaScript
- YAML
- `❯ JSON`

// will see this message:
Checking peerDependencies of eslint-config-airbnb-base@latest
The config that you've selected requires the following dependencies:

eslint-config-airbnb-base@latest eslint@^5.16.0 || ^6.8.0 || ^7.2.0 - eslint-plugin-import@^2.21.2

### ? Would you like to install them now with npm? No / › Yes`

- No
- `❯ Yes`

- You will also be asked to install extra packages. Choose `yes`.

---

## .eslintrc.json

"rules":
{"no-console": "off"}

---

## npm init

## npm install -D webpack webpack-cli

## npm install -D eslint prettier

## npm install -D eslint-config-prettier eslint-plugin-prettier

//or one line

## npm install -D webpack webpack-cli eslint prettier eslint-config-prettier eslint-plugin-prettier

## npx install-peerdeps --dev eslint-config-airbnb

## //in root

## touch .eslintrc.json .prettierrc webpack.config.js

## eslintrc content:

{
"extends": ["airbnb", "prettier"],
"env": {
"browser": true,
"node": true
}
}

## prettierrc content:

{
"printWidth": 100,
"singleQuote": true
}

---

.gitignore

> touch .gitignore && echo "node_modules/" >> .gitignore && git rm -r --cached node_modules ; git status

## package.json "scripts":{}

{
"test": "echo \"Error: no test specified\" && exit 1",
"watch": "webpack --watch",
"setup": "git subtree push --prefix dist/index.html origin gh-pages",
"deploy": "git subtree push --prefix dist origin gh-pages",
"build": "webpack"
}

## in webpack.config.js:

{"main": "script.js",}

## {copy paste the webpack.config.js file}

## .env value=key

## ^ no quotes
