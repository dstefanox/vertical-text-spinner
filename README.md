[![Build Status](https://travis-ci.org/dstefanox/vertical-text-spinner.svg?branch=master)](https://travis-ci.org/dstefanox/vertical-text-spinner)

# vertical-text-spinner

An Polymer element which shows text content which is animated when appearing/disappearing. Text gets replaced by new text which slides-in from above or below, while replaced text slides-out of the component through the bottom or the top of the component. 

## Demo
To get better idea about this component, check [live demo](http://dstefanox.github.io/vertical-text-spinner/components/vertical-text-spinner)


## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install vertical-text-spinner --save
```

## Usage

1. Import  Element:

    ```html
    <link rel="import" href="bower_components/vertical-text-spinner/vertical-text-spinner.html">
    ```

2. Place it on the page:

    ```html
    <vertical-text-spinner id="spinner" content="Initial text">
    </vertical-text-spinner>
    ```

3. Spin some new text into component from above/below:

    ```js
    var el = document.getElementById("spinner");
    el.spinUp("Spinning up!")
    el.spinDown("Spinning down!")
    ```

## Customization

Element uses absolute positioning of internal elements, so it is important understand how to style it.
By default, element has fixed height of 36 pixels, which corresponds to line height (this allows text to be centered verticaly within element).
To keep text verticaly centered within element, keep line height and element height same values.

The following custom properties are available for styling:

Custom property | Description | Default
----------------|-------------|----------
`--vertical-text-spinner-font-size` | Size of the font used to show text within element | `24px`
`--vertical-text-spinner-line-height` | Text line height. Keep it same value as element height to make text vertically centered | `36px`
`--vertical-text-spinner-height` | Height of the element | `36px`
`--vertical-text-spinner-color` | Text color | `black`
`--vertical-text-spinner-background-color` | Background color of the element | `{}`


## License

[MIT License](http://opensource.org/licenses/MIT)
