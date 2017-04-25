# \<validate-string\>
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/diddledan/validate-string)

Validate an input string and supply it to an output if it conforms to the test

## Installation
1. Install bower per their instructions, such as via:
    ```
    npm install -g bower
    ```
1. Using bower install the package to your project
    ```
    cd $YOUR_PROJECT_DIR
    bower install validate-string
    ```

You will now find a folder called bower_components in your project root which contains the webcomponents polyfill, and the validate-string element files along with any dependencies required.

## Usage
<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="validate-string.html">
    <link rel="import" href="../polymer/polymer.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<body>
  <template is="dom-bind">
    <validate-string input="string passes test" accepted-regex='passes' is-valid="{{passValid}}" output="{{pass}}"></validate-string>
    <p>First test is valid: [[passValid]]</p><p>First test output: [[pass]]</p>
    <validate-string input="string fails test" accepted-regex='passes' is-valid="{{failValid}}" output="{{fail}}"></validate-string>
    <p>Second test is valid: [[failValid]]</p><p>Second test output: [[fail]]</p>
  </template>
</body>
```

## Contributing
1. Fork it!
1. Create your feature branch: `git checkout -b my-new-feature`
1. Commit your changes: `git commit -am 'Add some feature'`
1. Push to the branch: `git push origin my-new-feature`
1. Submit a pull request :D

## History
* 0.0.2 Published onto webcomponents.org
* 0.0.1 Initial release published via bower

## Credits
* [Daniel Llewellyn (diddledan)](https://github.com/diddledan/)

## License
MIT License

See the `LICENSE` file in the root folder of this package.