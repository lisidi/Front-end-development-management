$mkdir webpack-demo && cd webpack-demo

$npm init -y

$npm install --save-dev webpack

$新建webpack.config.js

```JS
const path = require('path');

module.exports = {
  mode: 'development',
  entry: './src/index.js',
  output: {
    filename: 'bundle.js',
    path: path.resolve(__dirname, 'dist')
  }
};
```
$npx webpack --config webpack.config.js 

$修改package.json 

```JS
"scripts": {
    "build": "webpack"
 }
```
 $npm run build