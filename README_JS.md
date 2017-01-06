``````````````
babel,babel-preset-es2015

.babelrc file

//convert
babel es6.js

//run
babel-node es6.js
``````````````
webpack, babel-loader

//bundle with webpack for browser
webpack "./js/pie.js" "./dist/pie.js" --module-bind "js=babel-loader"

``````````````