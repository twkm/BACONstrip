
# BACON/strip Minimal CSS Framework

BACON/strip is a stripped-down responsive grid and front-end framework, ideal for making microsites and single-page sites without much overhead.

BACON/strip is also extremely customizable using [SASS](http://sass-lang.com/). You can specify the selectors you want to use including the grid container, rows, and columns, allowing you to customize your own grid selectors or retrofit an existing grid system.

## Installation

### Basic CSS

BACON/strip is precompiled using default variables in the [latest release](https://github.com/twkm/BACONstrip/releases/latest). You can simply include the `css/styles.css` stylesheet from the latest release to start using the grid and components. The breakpoint utilities plugin is precompiled in the css version of the framework.

### Sass

If you'd like to customize the variables and styles using Sass, you will need to copy the `scss/` directory from the [latest release](https://github.com/twkm/BACONstrip/releases/latest). Visit the [Sass website](http://sass-lang.com/) for instructions on installing and using Sass.

## Usage

To alter BACON/strip, import your webfonts and change any of the default values in `scss/styles.scss` before importing `BACON/strip`. All of the customizable values can be found in the `scss/BACON/base/_variables.scss` file.

Default `styles.scss`:

```PHP
// CUSTOM DEFINITIONS
// Create any custom definitions here, before the base files are loaded. 
// See the base/_variables.scss file for variables that can be set

// Example:
// $container-selector: '.bacontainer';
// $row-selector: '.row';
// $plugins-prefix: 'bit-';

@import url('https://fonts.googleapis.com/css?family=Raleway'); // Import Google Fonts

@import "BACON/strip";

// BACON/bits (Plugins) //
// @import "BACON/bits/nr-columns"; // Non-responsive columns plugin
@import "BACON/bits/breakpoint-utilities";
// @import "BACON/bits/rmedia-wrapper"; // Responsive media helper plugin

// Your styles go here...

```

Once you are happy with the style definitions in `styles.scss`, run Sass to compile your css and include the result in your project.

## Documentation

Learn more about how to use the default framework styling, or customize it using Sass, at <http://baconstrip.caliston.com>.
