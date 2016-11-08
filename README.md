## Babel
- Babel is a transpiler for 
  - ES.Next to ES5 transformation
  - JSX to ES5 transformation 
  - and more
- babel-cli is the CLI version of this tool (```npm install --save-dev babel-cli```)
- Need to explicitly specify the transformations that you want, no defaults.
  - Install:```npm install babel-preset-es2015 --save-dev```
  - Specify these presets in the .babelrc file as ```{'presets': ['es2015']}```
- Pro-tip 1: do not install global versions of babel because different versions maybe used by different projects
- Pro-tip 2: Instead of going to the nodde_modules directory to run babel, alias it as an npm task  in the package.json
- babel-loader is the webpack consumable version of babel
- Real-world projects typically use babel via webpack

## Webpack
- Starting with a user-specified entry point file, it builds a dependency graph, Concatenates and bundles all dependent files into one file
- Dont need a seperate babelrc, can use the query property in webpack.config.js to specify babel presets

### Process
1. Webpack loads Babel
2. Babel applies ES2015 transforms
3. Webpack bundles all the different JS files into one file

Complete the webpack tutorial at http://blog.madewithlove.be/post/webpack-your-bags/
