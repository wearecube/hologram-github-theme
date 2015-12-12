# Hologram Github Theme

This is a very simple [Github Styleguide](https://github.com/styleguide) inspired theme for Trulia's [Hologram](https://github.com/trulia/hologram), the ruby front-end doc generator.

## Preview

![Example](example.png?raw=true)

[Visit example styleguide](http://wearecube.github.io/hologram-github-theme-example/styleguide)

## Usage

Install Hologram:

```
$ gem install hologram
```

Add this theme to your project using NPM:

```
$ npm install --save-dev hologram-github-theme
```

Alternatively you may use Bower:

```
$ bower install --save-dev hologram-github-theme
```

Define the theme in your `hologram_config.yml`:

```
# Relative path(s) to your source files
source: app/styles

# Relative path where you want the documentation to be built
destination: styleguide

# The path that contains supporting assets for the documentation page
documentation_assets: node_modules/hologram-github-theme

# Category that will be used as the index.html (optional)
index: styleguide

# A list of relative paths to folders containing any dependencies to copy
dependencies:
  - 'dist'

# The CSS files to be included in the styleguide
css_include:
  - 'dist/styles/vendor.css'
  - 'dist/styles/main.css'

# The JavaScript files to included in the styleguide
js_include:
  - 'dist/scripts/main.js'

# The global title that is displayed at the top of the pages
global_title: Styleguide

```

In this example the markdown file `app/styles/styleguide.md` is used for the content on the index page. Also, if you're using Bower, adjust the package path accordingly: ```documentation_assets: bower_components/hologram-github-theme```.

For more details on the options, checkout the [Hologram documentation](https://github.com/trulia/hologram/blob/master/README.md#creating-a-yaml-config-file)

Finally, build the styleguide:

```
hologram -c hologram_config.yml
```

## Authors

The Hologram Github Theme has been created by [Mathis Hofer](https://github.com/hupf). Many thanks to [Maurice Kühlborn](https://github.com/minimalweb) and [Oscar](https://github.com/obartra) for their contributions.

## License

The Hologram Github Theme is licensed under the [MIT License](LICENSE)
