# webpack-survey

A deeper webpack study


_Foreword_

In this sruvey, I will review different aspects of web pack, un til I have enough informations, to to a first figure of this special character, in the front end world, that webpack is.

First, I will review the core, deppest prinicples I identifiy, through the different "primers" prensent in the webpack official docuementation. That will be in the [_Primer_](#primer) chapter.

## Primer

https://webpack.js.org/guides/getting-started/

> 
> ### Modules
> 
> The import and export statements have been standardized in ES2015. Although they are not supported in most browsers yet, webpack does support them out of the box.
> 
> Behind the scenes, webpack actually "transpiles" the code so that older browsers can also run it. If you inspect dist/main.js, you might be able to see how webpack does this, it's quite ingenious! Besides import and export, webpack supports various other module syntaxes as well, see Module API for more information.
> 
> Note that webpack will not alter any code other than import and export statements. If you are using other ES2015 features, make sure to use a transpiler such as Babel or Bublé via webpack's loader system.
> 
> 
> At its core, webpack is a static module bundler for modern JavaScript applications. When webpack processes your application, it internally builds a dependency graph which maps every module your project needs and generates one or more bundles

Here are the first lines, to keep, that are deep, in webpack docuementation  (comared to webpack's total depth, wwe'll hpoefully see deeper things, in our little humans life) : 

* `Webpack`'s first mentioned concern in official documentation is dependency management
* `Webpack` addresses dependency manngement, relying on some `ES2015` features : 
  * webpack knows how to read and write in `ES2015` language, if and only if what you use of `ES2015` is reduced to the two words (in the language theory terminology)  `import` and `export`.
  * the developer uses the `ES2015` to specify dependency relations between`ES2015` modules, at code edtion time,
  * webpack, at build time, compiles `ES2015` to whatever JavaScript the browser(s) supports.
  * You deploy what's produced by webapck build, to servers.
* webpack supports all browsers that are [ES5-compliant](https://kangax.github.io/compat-table/es5/) : 
  * `IE8` and below are not supported. 
  * webpack needs `Promise` for `import()` and `require.ensure()`. If you want to support older browsers, you will need to load a [`polyfill`](https://en.wikipedia.org/wiki/Polyfill_%28programming%29) before using these expressions.
Here you go.

> 
> ### `polyfill`
> 
> In web development, a polyfill is code that implements a feature on web browsers that do not support the feature.
> 
> wikipedia.
> 

_My Little thoughts_

* You should learn `TypeScript` with `Webpack`
* You should learn `Webpack` with `TypeScript`

