Direction CSS Framework
=======================

Lightweight CSS framework.

About this framework in a nutshell:
* Based on some parts of the Twitter Bootstap
* Includes only commonly used styles
* Uses LESS to be highly customizable (see `/style.example.less`)
* Provides a lot of useful mixins (see `css3.less`, `gradients.less`, etc)
* All class names in the framework are namespaced by `d-` to avoid collisions with other styles
* Included reset.css based on normalize.css implementation


## Installation

### Bower

Just run `bower install --save direction-css` - that's all!

### Manually

1. Download latest version of Direction CSS [here](https://github.com/Nodge/direction-css/releases)
2. Download latest version of Normalize.css [here](https://github.com/necolas/normalize.css/releases)
3. Update the path to Normalize.css in `css/dependencies.less`


## Usage

1. Copy the `style.example.less` and `config.example.less` to your css directory (remove `.example` suffix).
2. Include 'style.less` to your pages.
3. You can configure framework by editing `config.less` and `style.less`.
4. Include own less/css files in `style.less`.


## Framework classes (most of all)

### Common

* `.d-left` - Align content to left (including images)
* `.d-right` - Align content to right (including images)
* `.d-hide` - Alias for `display: none`

### Typography

* `.d-text` - Enable text styles for content inside the tag
* `.d-h1` and mixin `.d-h1()` - Style any element as H1
* `.d-h2` and mixin `.d-h2()` - Style any element as H2
* `.d-h3` and mixin `.d-h3()` - Style any element as H3
* `.d-h4` and mixin `.d-h4()` - Style any element as H4
* `.d-h5` and mixin `.d-h5()` - Style any element as H5
* `.d-h6` and mixin `.d-h6()` - Style any element as H6
* `.d-before-list` - Reduce bottom margin for paragraphs before lists
* `.d-list-unstyled` and mixin `.d-unstyle-list()` - Remove styles for the list
* `.d-list-unstyled-nested` and mixin `.d-unstyle-list-nested()` - Remove styles for the list and all nested lists
* `.d-table` - Apply special styles to the table
* `.d-table-condensed` - Make table more compact
* `.d-table-bordered` - Add borders to the table
* `.d-table-hover` - Add background color to the table's rows on hover
* `.d-table-striped` - Add background color to the table's odd/even rows
* `.d-table-responsive` - Wrap the table to `div.d-table-responsive` to enable horizontal scrolling on small screens

### Grid

Direction CSS Framework provides 24-columns fluid grid.

* `.d-container` - Wrap all contents to this container (provides centering, min/max width, page padding, etc)
* `.d-row` - Use this class to display columns in one line (can be nested)
* `.d-col-{n}` - Add this class to all columns (where `n` from 1 to 24)
* `.d-col-offset-{n}` - Add this class to create space between columns (where `n` from 1 to 24)
* `.d-col-pull-{n}` - Add this class to create space between columns (where `n` from 1 to 24)
* `.d-col-push-{n}` - Add this class to create space between columns (where `n` from 1 to 24)

### Forms

* `d-legend`
* `d-label` - Add this class to style labels
* `d-output`
* `d-required` - Use this class for required mark: `<span class="d-required">*</span>`
* `d-form-control` - Add this class to style any input (text, textarea, select, etc)
* `d-radio`
* `d-checkbox`
* `d-radio-inline`
* `d-checkbox-inline`
* `d-help-block`
* `d-form-warning`
* `d-form-error`
* `d-form-success`
* `d-form-group`
* `d-form-inline`
* `d-form-horizontal`

### Buttons

* `d-btn`
* `d-btn-disabled`
* `d-btn-block`
* `d-btn-link`
* `d-btn-default`
* `d-btn-primary`
* `d-btn-warning`
* `d-btn-danger`
* `d-btn-success`
* `d-btn-info`


## Build-in mixins

### Common

* `d-clearfix()`
* `d-text-overflow()` - Shortcut for `text-overflow` property (with required styles)
* `d-hide-text()` - Hide any text inside the tag but keep the tag itself visible
* `d-tab-focus()`
* `d-screen-reader()` - Only display content to screen readers

### Css3

* `d-border-radius(@radius)` - deprecated
* `d-box-shadow(@shadow)`
* `d-transition(@transition)`
* `d-transition-property(@transition-property)`
* `d-transition-delay(@transition-delay)`
* `d-transition-duration(@transition-duration)`
* `d-transform-transition(@transition)`
* `d-transform(@transform)`
* `d-rotate(@degrees)` - Shortcut for .d-transform
* `d-scale(@ratio)` - Shortcut for .d-transform
* `d-translate(@x: 0, @y: 0)` - Shortcut for .d-transform
* `d-translate3d(@x: 0, @y: 0, @z: 0)` - Shortcut for .d-transform
* `d-skew(@x: 0, @y: 0)` - Shortcut for .d-transform
* `d-flipH()` - Flip the element horizontally
* `d-transform-origin(@origin)`
* `d-animation(@animation)`
* `d-background-clip(@clip)`
* `d-background-size(@size)`
* `d-box-sizing(@boxmodel)`
* `d-user-select(@select)`
* `d-resizable(@direction: both)`
* `d-content-columns(@columnCount, @columnGap: @gridColumnGutter)`
* `d-hyphens(@mode: auto)`
* `d-opacity(@opacity)`
* `d-placeholder(@color)` - Set placeholder color for inputs

### Gradients

* `#d-gradient > .horizontal(@start-color, @end-color, @start-percent: 0%, @end-percent: 100%)`
* `#d-gradient > .horizontal-three-colors(@start-color, @mid-color, @color-stop, @end-color)`
* `#d-gradient > .vertical(@start-color, @end-color, @start-percent: 0%, @end-percent: 100%)`
* `#d-gradient > .vertical-bordered(@primaryColor, @secondaryColor)`
* `#d-gradient > .vertical-three-colors(@start-color, @mid-color, @color-stop, @end-color)`
* `#d-gradient > .directional(@start-color, @end-color, @deg: 45deg)`
* `#d-gradient > .radial(@inner-color, @outer-color)`
* `#d-gradient > .striped(@color: rgba(255,255,255,.15), @angle: 45deg)`

### Typography

* `d-h1()` - Style any element as H1
* `d-h2()` - Style any element as H2
* `d-h3()` - Style any element as H3
* `d-h4()` - Style any element as H4
* `d-h5()` - Style any element as H5
* `d-h6()` - Style any element as H6
* `d-unstyle-list()` - Remove styles for the list
* `d-unstyle-list-nested()` - Remove styles for the list and all nested lists
* `d-link-color(@color)` - Set link text color (including `:hover`, `:active` and `:visited` states)
* `d-link-color(@color, @color-hover)` - Set link text color (including `:hover`, `:active` and `:visited` states)
* `d-link-color(@color, @color-hover, @color-visited, @color-active)` - Set link text color (including `:hover`, `:active` and `:visited` states)
* `d-link-static-color(@color)` - Set the same link text color for all states (including `:hover`, `:active` and `:visited` states)
* `d-table-base()` - Apply special styles to the table
* `d-table-base > .condensed()` - Make table more compact
* `d-table-base > .bordered()` - Add borders to the table
* `d-table-base > .striped()` - Add background color to the table's odd/even rows
* `d-table-base > .hover()` - Add background color to the table's rows on hover

### IE

* `d-filter(@filter)`
* `d-ms-filter(@filter)`
* `d-reset-filter() `
* `d-zindex-bg-fix()` - Fix z-index bug on empty elements in IE8
