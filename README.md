Template for JS Projects
========

Implents ES2015 (w/ Babel), Webpack, Sass, Ava for testing, and Flow for type checking.

#### Resources
* [Ava: Futuristic test runner](https://github.com/avajs/ava)
* [React Ava Workshop](https://github.com/kentcdodds/react-ava-workshop/blob/master/INSTRUCTIONS.md)
* [Webpack Module Builder](https://webpack.github.io/docs/usage.html)
* [Sass Basics](http://sass-lang.com/guide)
* [Tutorial – write in ES6 and Sass on the front end with Webpack and Babel](http://tech.90min.com/?p=1340)
* [About Flow](https://flowtype.org/docs/about-flow.html)
* [Getting Started with Flow and Webpack](http://blog.iansinnott.com/getting-started-with-flow-and-webpack/)


Getting Started
---------------

1. clone: `git clone https://github.com/andybp85/GERasterCreator.git`
2. run `npm install` from the root directory.
3. set `NODE_ENV` in your environment and add your google maps api browser key to the apprpriate file in `confg` (see below)
4. run the dev server: `npm run dev`
5. run tests with `npm test`
6. check test coverage with `npm run chcoverage` and create coverage report with `npm run cover`
7. run typechecking with `flow`
8. have a look through `package.json` to see what else is going on (there's watch versons of previous commands, for starters)

Config
------

The npm scripts set a `NODE_ENV` environment varable, which is used to pick a config file in `config/`. Currently, they correspond to `config/development.js` and `config/test.js`. For now, both should contain the same info, a Google Maps API Browser key. Config files should look like this:
```js
export const YOUR_VAL='yourapikey';

```
