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

# Moby Dick

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> The text of _Moby Dick_ by Herman Melville.

<section class="intro">

</section>

<!-- /.intro -->



<section class="usage">

## Usage

```javascript
import text from 'https://cdn.jsdelivr.net/gh/stdlib-js/datasets-moby-dick@esm/index.mjs';
```
The previous example will load the latest bundled code from the esm branch. Alternatively, you may load a specific version by loading the file from one of the [tagged bundles](https://github.com/stdlib-js/datasets-moby-dick/tags). For example,

```javascript
import text from 'https://cdn.jsdelivr.net/gh/stdlib-js/datasets-moby-dick@v0.2.0-esm/index.mjs';
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

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="module">

import text from 'https://cdn.jsdelivr.net/gh/stdlib-js/datasets-moby-dick@esm/index.mjs';

var data;
var i;

data = text();
for ( i = 0; i < data.length; i++ ) {
    console.log( 'Character Count: %d', data[ i ].text.length );
}

</script>
</body>
</html>
```

</section>

<!-- /.examples -->



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

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## Copyright

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/datasets-moby-dick.svg
[npm-url]: https://npmjs.org/package/@stdlib/datasets-moby-dick

[test-image]: https://github.com/stdlib-js/datasets-moby-dick/actions/workflows/test.yml/badge.svg?branch=v0.2.0
[test-url]: https://github.com/stdlib-js/datasets-moby-dick/actions/workflows/test.yml?query=branch:v0.2.0

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/datasets-moby-dick/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/datasets-moby-dick?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/datasets-moby-dick.svg
[dependencies-url]: https://david-dm.org/stdlib-js/datasets-moby-dick/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[cli-section]: https://github.com/stdlib-js/datasets-moby-dick#cli
[cli-url]: https://github.com/stdlib-js/datasets-moby-dick/tree/cli
[@stdlib/datasets-moby-dick]: https://github.com/stdlib-js/datasets-moby-dick/tree/main

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/datasets-moby-dick/tree/deno
[deno-readme]: https://github.com/stdlib-js/datasets-moby-dick/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/datasets-moby-dick/tree/umd
[umd-readme]: https://github.com/stdlib-js/datasets-moby-dick/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/datasets-moby-dick/tree/esm
[esm-readme]: https://github.com/stdlib-js/datasets-moby-dick/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/datasets-moby-dick/blob/main/branches.md

[pddl-1.0]: http://opendatacommons.org/licenses/pddl/1.0/

[cc0]: https://creativecommons.org/publicdomain/zero/1.0

[apache-license]: https://www.apache.org/licenses/LICENSE-2.0

[ndjson]: http://specs.frictionlessdata.io/ndjson/

</section>

<!-- /.links -->
