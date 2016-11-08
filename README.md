## Babel
- Babel is a transpiler for 
  - JSX to ES5 transformation
  - ES.Next to ES5 transformation
  - and more
- babel-cli is the CLI version of this tool (```npm install --save-dev babel-cli```)
- Need to explicitly specify the transformations that you want, no defaults.
  - Eg. ```npm install babel-preset-es2015 react --save-dev```
- Pro-tip 1: do not install global versions of babel because different versions maybe used by different projects
- Pro-tip 2: Instead of going to the nodde_modules directory to run babel, alias it as an npm task  in the package.json
- babel-loader is the webpack consumable version of babel

## Webpack
Complete the webpack tutorial at http://blog.madewithlove.be/post/webpack-your-bags/
