# <img width="35" height="35" src="https://webpack.js.org/assets/icon-square-big.svg"> Webpack boilerplate
My boilerplate for webpack 5 with babel, eslint, prettier and [other plugins.](#file_folder-dependencies)

## :floppy_disk: Installation:
Clone this repository and install by typing:
``` bash
npm i
```

## :computer: Using:

Development server:
``` bash
npm run serve
```

Build:
``` bash
npm run build
```

Format all files by prettier:
``` bash
npm run format
```


## :abcd: Prettier & ESlint config:

.prettierrc
``` JSON
{
    "singleQuote": true,
    "printWidth": 100,
    "arrowParens": "avoid"
}
```

.eslintrc
``` JSON
{
    "extends": ["eslint:recommended", "plugin:prettier/recommended"],
    "plugins": ["prettier"],
    "rules": {
      "prettier/prettier": [
        "error",
        { "singleQuote": true, "printWidth": 100, "arrowParens": "avoid" }
      ],
      "arrow-parens": ["warn", "as-needed"]
    },
    "env": {
      "browser": true,
      "node": true,
      "es6": true
    },
    "parserOptions": {
      "sourceType": "module"
    },
    "parser": "babel-eslint"
}
```

## :file_folder: Dependencies:
```JSON
"devDependencies": {
    "@babel/core": "^7.15.0",
    "@babel/eslint-parser": "^7.15.0",
    "@babel/plugin-syntax-top-level-await": "^7.14.5",
    "@babel/plugin-transform-runtime": "^7.15.0",
    "@babel/preset-env": "^7.15.0",
    "@babel/runtime": "^7.15.3",
    "autoprefixer": "^10.3.1",
    "babel-eslint": "^10.1.0",
    "babel-loader": "^8.2.2",
    "css-loader": "^6.2.0",
    "eslint": "^7.32.0",
    "eslint-config-prettier": "^8.3.0",
    "eslint-plugin-prettier": "^3.4.0",
    "eslint-webpack-plugin": "^3.0.1",
    "html-webpack-plugin": "^5.3.2",
    "mini-css-extract-plugin": "^2.2.0",
    "postcss": "^8.3.6",
    "postcss-loader": "^6.1.1",
    "prettier": "^2.3.2",
    "sass": "^1.38.0",
    "sass-loader": "^12.1.0",
    "style-loader": "^3.2.1",
    "webpack": "^5.51.1",
    "webpack-cli": "^4.8.0",
    "webpack-dev-server": "^4.0.0"
  },
  "dependencies": {
    "normalize.css": "^8.0.1"
  }
```
