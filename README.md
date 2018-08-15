# Webpack dumbest config

1. Run "npm i webpack webpack-cli"
2. Create webpack.config.js

```javascript
const path = require('path');

module.exports = {
    entry: {
        'app': './src/index.js'                 //The entry point. Multiple entries can be specified
    },
    output: {
        filename: '[name].bundle.js',           //[name] is the name of the entry being bundled
        path: path.resolve(__dirname, 'dist')   //The absolute location for generating the bundle
    },
};
```

3. Run "npx webpack" or "npx webpack -p" or "npx webpack --watch"
4. The bundle is generated in the specified dist folder
