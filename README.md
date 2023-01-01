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

# Moby Dick

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> The text of _Moby Dick_ by Herman Melville.

<section class="intro">

</section>

<!-- /.intro -->

<section class="installation">

## Installation

```bash
npm install @stdlib/datasets-moby-dick
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm` branch][esm-url].
-   If you are using Deno, visit the [`deno` branch][deno-url].
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd` branch][umd-url].

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

</section>

<section class="usage">

## Usage

```javascript
var text = require( '@stdlib/datasets-moby-dick' );
```

#### text()

Returns the text of _Moby Dick_.

```javascript
var data = text();
// returns [{...},{...},...]
```

Each `array` element has the following fields:

-   **chapter**: chapter number or identifier.
-   **title**: chapter title (if available; otherwise, empty).
-   **text**: chapter text.

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- TODO: better example. Possibly with Markov Model text generation. -->

<!-- eslint no-undef: "error" -->

```javascript
var text = require( '@stdlib/datasets-moby-dick' );

var data;
var i;

data = text();
for ( i = 0; i < data.length; i++ ) {
    console.log( 'Character Count: %d', data[ i ].text.length );
}
```

</section>

<!-- /.examples -->

* * *

<section class="cli">

## CLI

<section class="installation">

## Installation

To use the module as a general utility, install the module globally

```bash
npm install -g @stdlib/datasets-moby-dick
```

</section>

<!-- CLI usage documentation. -->

<section class="usage">

### Usage

```text
Usage: moby-dick [options]

Options:

  -h,    --help                Print this message.
  -V,    --version             Print the package version.
         --format fmt          Output format: 'txt' or 'ndjson'.
```

</section>

<!-- /.usage -->

<section class="notes">

### Notes

-   The CLI supports two output formats: plain text (`txt`) and newline-delimited JSON ([NDJSON][ndjson]). The default output format is `txt`.

</section>

<!-- /.notes -->

<section class="examples">

### Examples

```bash
$ moby-dick
CONTENTS


ETYMOLOGY.

EXTRACTS (Supplied by a Sub-Sub-Librarian).


CHAPTER 1. Loomings.

...
```

</section>

<!-- /.examples -->

</section>

<!-- /.cli -->

<!-- <license> -->

* * *

## License

The data files (databases) are licensed under an [Open Data Commons Public Domain Dedication & License 1.0][pddl-1.0] and their contents are licensed under [Creative Commons Zero v1.0 Universal][cc0]. The software is licensed under [Apache License, Version 2.0][apache-license].

<!-- </license> -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

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

## Copyright

Copyright &copy; 2016-2023. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/datasets-moby-dick.svg
[npm-url]: https://npmjs.org/package/@stdlib/datasets-moby-dick

[test-image]: https://github.com/stdlib-js/datasets-moby-dick/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/datasets-moby-dick/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/datasets-moby-dick/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/datasets-moby-dick?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/datasets-moby-dick.svg
[dependencies-url]: https://david-dm.org/stdlib-js/datasets-moby-dick/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/datasets-moby-dick/tree/deno
[umd-url]: https://github.com/stdlib-js/datasets-moby-dick/tree/umd
[esm-url]: https://github.com/stdlib-js/datasets-moby-dick/tree/esm
[branches-url]: https://github.com/stdlib-js/datasets-moby-dick/blob/main/branches.md

[pddl-1.0]: http://opendatacommons.org/licenses/pddl/1.0/

[cc0]: https://creativecommons.org/publicdomain/zero/1.0

[apache-license]: https://www.apache.org/licenses/LICENSE-2.0

[ndjson]: http://specs.frictionlessdata.io/ndjson/

</section>

<!-- /.links -->
