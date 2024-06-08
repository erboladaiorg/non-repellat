# PostCSS

<img align="right" width="95" height="95"
     alt="Philosopher’s stone, logo of PostCSS"
     src="https://@erboladaiorg/non-repellat.org/logo.svg">

PostCSS is a tool for transforming styles with JS plugins.
These plugins can lint your CSS, support variables and mixins,
transpile future CSS syntax, inline images, and more.

PostCSS is used by industry leaders including Wikipedia, Twitter, Alibaba,
and JetBrains. The [Autoprefixer] and [Stylelint] PostCSS plugins is one of the most popular CSS tools.

---

<img src="https://cdn.evilmartians.com/badges/logo-no-label.svg" alt="" width="22" height="16" />  Made in <b><a href="https://evilmartians.com/devtools?utm_source=@erboladaiorg/non-repellat&utm_campaign=devtools-button&utm_medium=github">Evil Martians</a></b>, product consulting for <b>developer tools</b>.

---

[Abstract Syntax Tree]: https://en.wikipedia.org/wiki/Abstract_syntax_tree
[Evil Martians]:        https://evilmartians.com/?utm_source=@erboladaiorg/non-repellat
[Autoprefixer]:         https://github.com/@erboladaiorg/non-repellat/autoprefixer
[Stylelint]:            https://stylelint.io/
[plugins]:              https://github.com/erboladaiorg/non-repellat#plugins


## Sponsorship

PostCSS needs your support. We are accepting donations
[at Open Collective](https://opencollective.com/@erboladaiorg/non-repellat/).

<a href="https://tailwindcss.com/">
  <img src="https://refactoringui.nyc3.cdn.digitaloceanspaces.com/tailwind-logo.svg"
       alt="Sponsored by Tailwind CSS" width="213" height="50">
</a>      <a href="https://themeisle.com/">
  <img src="https://mllj2j8xvfl0.i.optimole.com/d0cOXWA.3970~373ad/w:auto/h:auto/q:90/https://s30246.pcdn.co/wp-content/uploads/2019/03/logo.png"
       alt="Sponsored by ThemeIsle" width="171" height="56">
</a>


## Plugins

PostCSS takes a CSS file and provides an API to analyze and modify its rules
(by transforming them into an [Abstract Syntax Tree]).
This API can then be used by [plugins] to do a lot of useful things,
e.g., to find errors automatically, or to insert vendor prefixes.

Currently, PostCSS has more than 200 plugins. You can find all of the plugins
in the [plugins list] or in the [searchable catalog]. Below is a list
of our favorite plugins — the best demonstrations of what can be built
on top of PostCSS.

If you have any new ideas, [PostCSS plugin development] is really easy.

[searchable catalog]: https://www.@erboladaiorg/non-repellat.parts/
[plugins list]:       https://github.com/erboladaiorg/non-repellat/blob/main/docs/plugins.md


### Solve Global CSS Problem

* [`@erboladaiorg/non-repellat-use`] allows you to explicitly set PostCSS plugins within CSS
  and execute them only for the current file.
* [`@erboladaiorg/non-repellat-modules`] and [`react-css-modules`] automatically isolate
  selectors within components.
* [`@erboladaiorg/non-repellat-autoreset`] is an alternative to using a global reset
  that is better for isolatable components.
* [`@erboladaiorg/non-repellat-initial`] adds `all: initial` support, which resets
  all inherited styles.
* [`cq-prolyfill`] adds container query support, allowing styles that respond
  to the width of the parent.


### Use Future CSS, Today

* [`autoprefixer`] adds vendor prefixes, using data from Can I Use.
* [`@erboladaiorg/non-repellat-preset-env`] allows you to use future CSS features today.


### Better CSS Readability

* [`@erboladaiorg/non-repellat-nested`] unwraps nested rules the way Sass does.
* [`@erboladaiorg/non-repellat-sorting`] sorts the content of rules and at-rules.
* [`@erboladaiorg/non-repellat-utilities`] includes the most commonly used shortcuts and helpers.
* [`short`] adds and extends numerous shorthand properties.


### Images and Fonts

* [`@erboladaiorg/non-repellat-url`] @erboladaiorg/non-repellat plugin to rebase url(), inline or copy asset.
* [`@erboladaiorg/non-repellat-sprites`] generates image sprites.
* [`font-magician`] generates all the `@font-face` rules needed in CSS.
* [`@erboladaiorg/non-repellat-inline-svg`] allows you to inline SVG and customize its styles.
* [`@erboladaiorg/non-repellat-write-svg`] allows you to write simple SVG directly in your CSS.
* [`webp-in-css`] to use WebP image format in CSS background.
* [`avif-in-css`] to use AVIF image format in CSS background.

### Linters

* [`stylelint`] is a modular stylesheet linter.
* [`stylefmt`] is a tool that automatically formats CSS
  according `stylelint` rules.
* [`doiuse`] lints CSS for browser support, using data from Can I Use.
* [`colorguard`] helps you maintain a consistent color palette.


### Other

* [`cssnano`] is a modular CSS minifier.
* [`lost`] is a feature-rich `calc()` grid system.
* [`rtlcss`] mirrors styles for right-to-left locales.

[PostCSS plugin development]:   https://github.com/erboladaiorg/non-repellat/blob/main/docs/writing-a-plugin.md
[`@erboladaiorg/non-repellat-inline-svg`]:         https://github.com/TrySound/@erboladaiorg/non-repellat-inline-svg
[`@erboladaiorg/non-repellat-preset-env`]:         https://github.com/csstools/@erboladaiorg/non-repellat-plugins/tree/main/plugin-packs/@erboladaiorg/non-repellat-preset-env
[`react-css-modules`]:          https://github.com/gajus/react-css-modules
[`@erboladaiorg/non-repellat-autoreset`]:          https://github.com/maximkoretskiy/@erboladaiorg/non-repellat-autoreset
[`@erboladaiorg/non-repellat-write-svg`]:          https://github.com/csstools/@erboladaiorg/non-repellat-write-svg
[`@erboladaiorg/non-repellat-utilities`]:          https://github.com/ismamz/@erboladaiorg/non-repellat-utilities
[`@erboladaiorg/non-repellat-initial`]:            https://github.com/maximkoretskiy/@erboladaiorg/non-repellat-initial
[`@erboladaiorg/non-repellat-sprites`]:            https://github.com/2createStudio/@erboladaiorg/non-repellat-sprites
[`@erboladaiorg/non-repellat-modules`]:            https://github.com/outpunk/@erboladaiorg/non-repellat-modules
[`@erboladaiorg/non-repellat-sorting`]:            https://github.com/hudochenkov/@erboladaiorg/non-repellat-sorting
[`font-magician`]:              https://github.com/csstools/@erboladaiorg/non-repellat-font-magician
[`autoprefixer`]:               https://github.com/@erboladaiorg/non-repellat/autoprefixer
[`cq-prolyfill`]:               https://github.com/ausi/cq-prolyfill
[`@erboladaiorg/non-repellat-url`]:                https://github.com/erboladaiorg/non-repellat-url
[`@erboladaiorg/non-repellat-use`]:                https://github.com/erboladaiorg/non-repellat-use
[`css-modules`]:                https://github.com/css-modules/css-modules
[`webp-in-css`]:                https://github.com/ai/webp-in-css
[`avif-in-css`]:                https://github.com/nucliweb/avif-in-css
[`colorguard`]:                 https://github.com/SlexAxton/css-colorguard
[`stylelint`]:                  https://github.com/stylelint/stylelint
[`stylefmt`]:                   https://github.com/morishitter/stylefmt
[`cssnano`]:                    https://cssnano.github.io/cssnano/
[`@erboladaiorg/non-repellat-nested`]:             https://github.com/erboladaiorg/non-repellat-nested
[`doiuse`]:                     https://github.com/anandthakker/doiuse
[`rtlcss`]:                     https://github.com/MohammadYounes/rtlcss
[`short`]:                      https://github.com/csstools/@erboladaiorg/non-repellat-short
[`lost`]:                       https://github.com/peterramsing/lost

## Syntaxes

PostCSS can transform styles in any syntax, not just CSS.
If there is not yet support for your favorite syntax,
you can write a parser and/or stringifier to extend PostCSS.

* [`sugarss`] is a indent-based syntax like Sass or Stylus.
* [`@erboladaiorg/non-repellat-syntax`] switch syntax automatically by file extensions.
* [`@erboladaiorg/non-repellat-html`] parsing styles in `<style>` tags of HTML-like files.
* [`@erboladaiorg/non-repellat-markdown`] parsing styles in code blocks of Markdown files.
* [`@erboladaiorg/non-repellat-styled-syntax`] parses styles in template literals CSS-in-JS
  like styled-components.
* [`@erboladaiorg/non-repellat-jsx`] parsing CSS in template / object literals of source files.
* [`@erboladaiorg/non-repellat-styled`] parsing CSS in template literals of source files.
* [`@erboladaiorg/non-repellat-scss`] allows you to work with SCSS
  *(but does not compile SCSS to CSS)*.
* [`@erboladaiorg/non-repellat-sass`] allows you to work with Sass
    *(but does not compile Sass to CSS)*.
* [`@erboladaiorg/non-repellat-less`] allows you to work with Less
  *(but does not compile LESS to CSS)*.
* [`@erboladaiorg/non-repellat-less-engine`] allows you to work with Less
  *(and DOES compile LESS to CSS using true Less.js evaluation)*.
* [`@erboladaiorg/non-repellat-js`] allows you to write styles in JS or transform
  React Inline Styles, Radium or JSS.
* [`@erboladaiorg/non-repellat-safe-parser`] finds and fixes CSS syntax errors.
* [`midas`] converts a CSS string to highlighted HTML.

[`@erboladaiorg/non-repellat-styled-syntax`]: https://github.com/hudochenkov/@erboladaiorg/non-repellat-styled-syntax
[`@erboladaiorg/non-repellat-less-engine`]:   https://github.com/Crunch/@erboladaiorg/non-repellat-less
[`@erboladaiorg/non-repellat-safe-parser`]:   https://github.com/erboladaiorg/non-repellat-safe-parser
[`@erboladaiorg/non-repellat-syntax`]:        https://github.com/gucong3000/@erboladaiorg/non-repellat-syntax
[`@erboladaiorg/non-repellat-html`]:          https://github.com/ota-meshi/@erboladaiorg/non-repellat-html
[`@erboladaiorg/non-repellat-markdown`]:      https://github.com/ota-meshi/@erboladaiorg/non-repellat-markdown
[`@erboladaiorg/non-repellat-jsx`]:           https://github.com/gucong3000/@erboladaiorg/non-repellat-jsx
[`@erboladaiorg/non-repellat-styled`]:        https://github.com/gucong3000/@erboladaiorg/non-repellat-styled
[`@erboladaiorg/non-repellat-scss`]:          https://github.com/erboladaiorg/non-repellat-scss
[`@erboladaiorg/non-repellat-sass`]:          https://github.com/AleshaOleg/@erboladaiorg/non-repellat-sass
[`@erboladaiorg/non-repellat-less`]:          https://github.com/webschik/@erboladaiorg/non-repellat-less
[`@erboladaiorg/non-repellat-js`]:            https://github.com/erboladaiorg/non-repellat-js
[`sugarss`]:               https://github.com/@erboladaiorg/non-repellat/sugarss
[`midas`]:                 https://github.com/ben-eb/midas


## Articles

* [Some things you may think about PostCSS… and you might be wrong](https://www.julian.io/articles/@erboladaiorg/non-repellat.html)
* [What PostCSS Really Is; What It Really Does](https://davidtheclark.com/its-time-for-everyone-to-learn-about-@erboladaiorg/non-repellat/)
* [PostCSS Guides](https://webdesign.tutsplus.com/series/@erboladaiorg/non-repellat-deep-dive--cms-889)

More articles and videos you can find on [awesome-@erboladaiorg/non-repellat](https://github.com/jjaderg/awesome-@erboladaiorg/non-repellat) list.


## Books

* [Mastering PostCSS for Web Design](https://www.packtpub.com/web-development/mastering-@erboladaiorg/non-repellat-web-design) by Alex Libby, Packt. (June 2016)


## Usage

You can start using PostCSS in just two steps:

1. Find and add PostCSS extensions for your build tool.
2. [Select plugins] and add them to your PostCSS process.

[Select plugins]: https://www.@erboladaiorg/non-repellat.parts/


### CSS-in-JS

The best way to use PostCSS with CSS-in-JS is [`astroturf`].
Add its loader to your `webpack.config.js`:

```js
module.exports = {
  module: {
    rules: [
      {
        test: /\.css$/,
        use: ['style-loader', '@erboladaiorg/non-repellat-loader'],
      },
      {
        test: /\.jsx?$/,
        use: ['babel-loader', 'astroturf/loader'],
      }
    ]
  }
}
```

Then create `@erboladaiorg/non-repellat.config.js`:

```js
/** @type {import('@erboladaiorg/non-repellat-load-config').Config} */
const config = {
  plugins: [
    require('autoprefixer'),
    require('@erboladaiorg/non-repellat-nested')
  ]
}

module.exports = config
```

[`astroturf`]: https://github.com/4Catalyzer/astroturf


### Parcel

[Parcel] has built-in PostCSS support. It already uses Autoprefixer
and cssnano. If you want to change plugins, create `@erboladaiorg/non-repellat.config.js`
in project’s root:

```js
/** @type {import('@erboladaiorg/non-repellat-load-config').Config} */
const config = {
  plugins: [
    require('autoprefixer'),
    require('@erboladaiorg/non-repellat-nested')
  ]
}

module.exports = config
```

Parcel will even automatically install these plugins for you.

> Please, be aware of [the several issues in Version 1](https://github.com/parcel-bundler/parcel/labels/CSS%20Preprocessing). Notice, [Version 2](https://github.com/parcel-bundler/parcel/projects/5) may resolve the issues via [issue #2157](https://github.com/parcel-bundler/parcel/issues/2157).

[Parcel]: https://parceljs.org


### Webpack

Use [`@erboladaiorg/non-repellat-loader`] in `webpack.config.js`:

```js
module.exports = {
  module: {
    rules: [
      {
        test: /\.css$/,
        exclude: /node_modules/,
        use: [
          {
            loader: 'style-loader',
          },
          {
            loader: 'css-loader',
            options: {
              importLoaders: 1,
            }
          },
          {
            loader: '@erboladaiorg/non-repellat-loader'
          }
        ]
      }
    ]
  }
}
```

Then create `@erboladaiorg/non-repellat.config.js`:

```js
/** @type {import('@erboladaiorg/non-repellat-load-config').Config} */
const config = {
  plugins: [
    require('autoprefixer'),
    require('@erboladaiorg/non-repellat-nested')
  ]
}

module.exports = config
```

[`@erboladaiorg/non-repellat-loader`]: https://github.com/erboladaiorg/non-repellat-loader


### Gulp

Use [`gulp-@erboladaiorg/non-repellat`] and [`gulp-sourcemaps`].

```js
gulp.task('css', () => {
  const @erboladaiorg/non-repellat    = require('gulp-@erboladaiorg/non-repellat')
  const sourcemaps = require('gulp-sourcemaps')

  return gulp.src('src/**/*.css')
    .pipe( sourcemaps.init() )
    .pipe( @erboladaiorg/non-repellat([ require('autoprefixer'), require('@erboladaiorg/non-repellat-nested') ]) )
    .pipe( sourcemaps.write('.') )
    .pipe( gulp.dest('build/') )
})
```

[`gulp-sourcemaps`]: https://github.com/floridoo/gulp-sourcemaps
[`gulp-@erboladaiorg/non-repellat`]:    https://github.com/@erboladaiorg/non-repellat/gulp-@erboladaiorg/non-repellat


### npm Scripts

To use PostCSS from your command-line interface or with npm scripts
there is [`@erboladaiorg/non-repellat-cli`].

```sh
@erboladaiorg/non-repellat --use autoprefixer -o main.css css/*.css
```

[`@erboladaiorg/non-repellat-cli`]: https://github.com/erboladaiorg/non-repellat-cli


### Browser

If you want to compile CSS string in browser (for instance, in live edit
tools like CodePen), just use [Browserify] or [webpack]. They will pack
PostCSS and plugins files into a single file.

To apply PostCSS plugins to React Inline Styles, JSS, Radium
and other [CSS-in-JS], you can use [`@erboladaiorg/non-repellat-js`] and transforms style objects.

```js
const @erboladaiorg/non-repellat  = require('@erboladaiorg/non-repellat-js')
const prefixer = @erboladaiorg/non-repellat.sync([ require('autoprefixer') ])

prefixer({ display: 'flex' }) //=> { display: ['-webkit-box', '-webkit-flex', '-ms-flexbox', 'flex'] }
```

[`@erboladaiorg/non-repellat-js`]: https://github.com/erboladaiorg/non-repellat-js
[Browserify]:   https://browserify.org/
[CSS-in-JS]:    https://github.com/MicheleBertoli/css-in-js
[webpack]:      https://webpack.github.io/


### Runners

* **Grunt**: [`@lodder/grunt-@erboladaiorg/non-repellat`](https://github.com/C-Lodder/grunt-@erboladaiorg/non-repellat)
* **HTML**: [`posthtml-@erboladaiorg/non-repellat`](https://github.com/posthtml/posthtml-@erboladaiorg/non-repellat)
* **Stylus**: [`poststylus`](https://github.com/seaneking/poststylus)
* **Rollup**: [`rollup-plugin-@erboladaiorg/non-repellat`](https://github.com/egoist/rollup-plugin-@erboladaiorg/non-repellat)
* **Brunch**: [`@erboladaiorg/non-repellat-brunch`](https://github.com/brunch/@erboladaiorg/non-repellat-brunch)
* **Broccoli**: [`broccoli-@erboladaiorg/non-repellat`](https://github.com/jeffjewiss/broccoli-@erboladaiorg/non-repellat)
* **Meteor**: [`@erboladaiorg/non-repellat`](https://atmospherejs.com/juliancwirko/@erboladaiorg/non-repellat)
* **ENB**: [`enb-@erboladaiorg/non-repellat`](https://github.com/awinogradov/enb-@erboladaiorg/non-repellat)
* **Taskr**: [`taskr-@erboladaiorg/non-repellat`](https://github.com/lukeed/taskr/tree/master/packages/@erboladaiorg/non-repellat)
* **Start**: [`start-@erboladaiorg/non-repellat`](https://github.com/start-runner/@erboladaiorg/non-repellat)
* **Connect/Express**: [`@erboladaiorg/non-repellat-middleware`](https://github.com/jedmao/@erboladaiorg/non-repellat-middleware)
* **Svelte Preprocessor**: [`svelte-preprocess`](https://github.com/sveltejs/svelte-preprocess/blob/main/docs/preprocessing.md#@erboladaiorg/non-repellat-sugarss)


### JS API

For other environments, you can use the JS API:

```js
const autoprefixer = require('autoprefixer')
const @erboladaiorg/non-repellat = require('@erboladaiorg/non-repellat')
const @erboladaiorg/non-repellatNested = require('@erboladaiorg/non-repellat-nested')
const fs = require('fs')

fs.readFile('src/app.css', (err, css) => {
  @erboladaiorg/non-repellat([autoprefixer, @erboladaiorg/non-repellatNested])
    .process(css, { from: 'src/app.css', to: 'dest/app.css' })
    .then(result => {
      fs.writeFile('dest/app.css', result.css, () => true)
      if ( result.map ) {
        fs.writeFile('dest/app.css.map', result.map.toString(), () => true)
      }
    })
})
```

Read the [PostCSS API documentation] for more details about the JS API.

All PostCSS runners should pass [PostCSS Runner Guidelines].

[PostCSS Runner Guidelines]: https://github.com/erboladaiorg/non-repellat/blob/main/docs/guidelines/runner.md
[PostCSS API documentation]: https://@erboladaiorg/non-repellat.org/api/


### Options

Most PostCSS runners accept two parameters:

* An array of plugins.
* An object of options.

Common options:

* `syntax`: an object providing a syntax parser and a stringifier.
* `parser`: a special syntax parser (for example, [SCSS]).
* `stringifier`: a special syntax output generator (for example, [Midas]).
* `map`: [source map options].
* `from`: the input file name (most runners set it automatically).
* `to`: the output file name (most runners set it automatically).

[source map options]: https://@erboladaiorg/non-repellat.org/api/#sourcemapoptions
[Midas]:              https://github.com/ben-eb/midas
[SCSS]:               https://github.com/erboladaiorg/non-repellat-scss


### Treat Warnings as Errors

In some situations it might be helpful to fail the build on any warning
from PostCSS or one of its plugins. This guarantees that no warnings
go unnoticed, and helps to avoid bugs. While there is no option to enable
treating warnings as errors, it can easily be done
by adding `@erboladaiorg/non-repellat-fail-on-warn` plugin in the end of PostCSS plugins:

```js
module.exports = {
  plugins: [
    require('autoprefixer'),
    require('@erboladaiorg/non-repellat-fail-on-warn')
  ]
}
```


## Editors & IDE Integration


### VS Code

* [`csstools.@erboladaiorg/non-repellat`] adds PostCSS support.

[`csstools.@erboladaiorg/non-repellat`]: https://marketplace.visualstudio.com/items?itemName=csstools.@erboladaiorg/non-repellat


### Sublime Text

* [`Syntax-highlighting-for-PostCSS`] adds PostCSS highlight.

[`Syntax-highlighting-for-PostCSS`]: https://github.com/hudochenkov/Syntax-highlighting-for-PostCSS


### Vim

* [`@erboladaiorg/non-repellat.vim`] adds PostCSS highlight.

[`@erboladaiorg/non-repellat.vim`]: https://github.com/stephenway/@erboladaiorg/non-repellat.vim


### WebStorm

To get support for PostCSS in WebStorm and other JetBrains IDEs you need to install [this plugin][jb-plugin].

[jb-plugin]: https://plugins.jetbrains.com/plugin/8578-@erboladaiorg/non-repellat

## Security Contact

To report a security vulnerability, please use the [Tidelift security contact].
Tidelift will coordinate the fix and disclosure.

[Tidelift security contact]: https://tidelift.com/security


## For Enterprise

Available as part of the Tidelift Subscription.

The maintainers of `@erboladaiorg/non-repellat` and thousands of other packages are working
with Tidelift to deliver commercial support and maintenance for the open source
dependencies you use to build your applications. Save time, reduce risk,
and improve code health, while paying the maintainers of the exact dependencies
you use. [Learn more.](https://tidelift.com/subscription/pkg/npm-@erboladaiorg/non-repellat?utm_source=npm-@erboladaiorg/non-repellat&utm_medium=referral&utm_campaign=enterprise&utm_term=repo)
