<!--

@license Apache-2.0

Copyright (c) 2024 The Stdlib Authors.

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

# Modulus Function

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Evaluate the [Modulus function][modulus-function] for single-precision floating-point numbers.

<section class="intro">

The [modulus function][modulus-function] is defined as

<!-- <equation class="equation" label="eq:modulus_function" align="center" raw="z = x%y" alt="Modulus function"> -->

```math
z = x%y
```

<!-- </equation> -->

where `x` is the **dividend** and `y` is the **divisor**.

</section>

<!-- /.intro -->



<section class="usage">

## Usage

```javascript
import fmodf from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-fmodf@deno/mod.js';
```

#### fmodf( x, y )

Evaluates the [Modulus function][modulus-function] for single-precision floating-point numbers.

```javascript
var v = fmodf( 8.0, 3.0 );
// returns 2.0

v = fmodf( 9.0, 3.0 );
// returns 0.0

v = fmodf( 8.9, 3.0 );
// returns ~2.9

v = fmodf( NaN, 3.0 );
// returns NaN

v = fmodf( 5.0, NaN );
// returns NaN

v = fmodf( NaN, NaN );
// returns NaN
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
import discreteUniform from 'https://cdn.jsdelivr.net/gh/stdlib-js/random-array-discrete-uniform@deno/mod.js';
import fmodf from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-fmodf@deno/mod.js';

var x = discreteUniform( 10, 0.0, 100.0 );
var y = discreteUniform( 10, -50.0, 50.0 );
var i;

for ( i = 0; i < 10; i++ ) {
    console.log( '%f%%%f = %f', x[ i ], y[ i ], fmodf( x[ i ], y[ i ] ) );
}
```

</section>

<!-- /.examples -->

<!-- C interface documentation. -->



<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## Copyright

Copyright &copy; 2016-2025. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-fmodf.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-fmodf

[test-image]: https://github.com/stdlib-js/math-base-special-fmodf/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/math-base-special-fmodf/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-fmodf/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-fmodf?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-fmodf.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-fmodf/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-special-fmodf/tree/deno
[deno-readme]: https://github.com/stdlib-js/math-base-special-fmodf/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/math-base-special-fmodf/tree/umd
[umd-readme]: https://github.com/stdlib-js/math-base-special-fmodf/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/math-base-special-fmodf/tree/esm
[esm-readme]: https://github.com/stdlib-js/math-base-special-fmodf/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/math-base-special-fmodf/blob/main/branches.md

[modulus-function]: https://en.wikipedia.org/wiki/Remainder

<!-- <related-links> -->

<!-- </related-links> -->

</section>

<!-- /.links -->
