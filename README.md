<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# isPrimitive

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Test if a value is a JavaScript primitive.



<section class="usage">

## Usage

To use in Observable,

```javascript
isPrimitive = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-primitive@umd/browser.js' )
```
The previous example will load the latest bundled code from the umd branch. Alternatively, you may load a specific version by loading the file from one of the [tagged bundles](https://github.com/stdlib-js/assert-is-primitive/tags). For example,

```javascript
isPrimitive = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-primitive@v0.2.1-umd/browser.js' )
```

To vendor stdlib functionality and avoid installing dependency trees for Node.js, you can use the UMD server build:

```javascript
var isPrimitive = require( 'path/to/vendor/umd/assert-is-primitive/index.js' )
```

To include the bundle in a webpage,

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-primitive@umd/browser.js"></script>
```

If no recognized module system is present, access bundle contents via the global scope:

```html
<script type="text/javascript">
(function () {
    window.isPrimitive;
})();
</script>
```

#### isPrimitive( value )

Tests if a `value` is a JavaScript primitive.

```javascript
var bool = isPrimitive( false );
// returns true
```

</section>

<!-- /.usage -->

<section class="notes">

## Notes

-   Seven primitives:

    -   `string`
    -   `number`
    -   `boolean`
    -   `null`
    -   `undefined`
    -   `symbol` (ES6/ES2015)
    -   `bigint` (ES11/ES2020)

</section>

<!-- /.notes -->

<section class="examples">

## Examples

<!-- eslint-disable no-restricted-syntax, no-new-wrappers, no-empty-function, no-array-constructor -->

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/boolean-ctor@umd/browser.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/object-ctor@umd/browser.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-primitive@umd/browser.js"></script>
<script type="text/javascript">
(function () {

var bool = isPrimitive( false );
// returns true

bool = isPrimitive( 0 );
// returns true

bool = isPrimitive( '' );
// returns true

bool = isPrimitive( null );
// returns true

bool = isPrimitive( void 0 );
// returns true

bool = isPrimitive( [] );
// returns false

bool = isPrimitive( {} );
// returns false

bool = isPrimitive( function noop() {} );
// returns false

bool = isPrimitive( new Boolean() );
// returns false

bool = isPrimitive( new String() );
// returns false

bool = isPrimitive( new Array() );
// returns false

bool = isPrimitive( new Object() );
// returns false

})();
</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/assert-is-boxed-primitive`][@stdlib/assert/is-boxed-primitive]</span><span class="delimiter">: </span><span class="description">test if a value is a JavaScript boxed primitive.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/assert-is-primitive.svg
[npm-url]: https://npmjs.org/package/@stdlib/assert-is-primitive

[test-image]: https://github.com/stdlib-js/assert-is-primitive/actions/workflows/test.yml/badge.svg?branch=v0.2.1
[test-url]: https://github.com/stdlib-js/assert-is-primitive/actions/workflows/test.yml?query=branch:v0.2.1

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/assert-is-primitive/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/assert-is-primitive?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/assert-is-primitive.svg
[dependencies-url]: https://david-dm.org/stdlib-js/assert-is-primitive/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/assert-is-primitive/tree/deno
[deno-readme]: https://github.com/stdlib-js/assert-is-primitive/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/assert-is-primitive/tree/umd
[umd-readme]: https://github.com/stdlib-js/assert-is-primitive/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/assert-is-primitive/tree/esm
[esm-readme]: https://github.com/stdlib-js/assert-is-primitive/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/assert-is-primitive/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/assert-is-primitive/main/LICENSE

<!-- <related-links> -->

[@stdlib/assert/is-boxed-primitive]: https://github.com/stdlib-js/assert-is-boxed-primitive/tree/umd

<!-- </related-links> -->

</section>

<!-- /.links -->
