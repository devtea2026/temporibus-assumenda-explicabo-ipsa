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

# ndarray

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Multidimensional arrays.

<section class="installation">

## Installation

```bash
npm install @devtea2026/temporibus-assumenda-explicabo-ipsa
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm`][esm-url] branch (see [README][esm-readme]).
-   If you are using Deno, visit the [`deno`][deno-url] branch (see [README][deno-readme] for usage intructions).
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd`][umd-url] branch (see [README][umd-readme]).

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

To view installation and usage instructions specific to each branch build, be sure to explicitly navigate to the respective README files on each branch, as linked to above.

</section>

<section class="usage">

## Usage

```javascript
var ns = require( '@devtea2026/temporibus-assumenda-explicabo-ipsa' );
```

#### ns

ndarray namespace.

```javascript
var o = ns;
// returns {...}
```

The namespace exports the following functions to create multidimensional arrays:

<!-- <toc pattern="+(array|ctor)"> -->

<div class="namespace-toc">

-   <span class="signature">[`array( [buffer,] [options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/array]</span><span class="delimiter">: </span><span class="description">create a multidimensional array.</span>
-   <span class="signature">[`ndarray( dtype, buffer, shape, strides, offset, order[, options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/ctor]</span><span class="delimiter">: </span><span class="description">multidimensional array constructor.</span>

</div>

<!-- </toc> -->

The namespace contains the following sub-namespaces:

<!-- <toc pattern="+(base|iter)"> -->

<div class="namespace-toc">

-   <span class="signature">[`base`][@devtea2026/temporibus-assumenda-explicabo-ipsa/base]</span><span class="delimiter">: </span><span class="description">base ndarray.</span>
-   <span class="signature">[`iter`][@devtea2026/temporibus-assumenda-explicabo-ipsa/iter]</span><span class="delimiter">: </span><span class="description">multidimensional array iterators.</span>

</div>

<!-- </toc> -->

In addition, the namespace contains the following multidimensional array utility functions:

<!-- <toc pattern="*" > -->

<div class="namespace-toc">

-   <span class="signature">[`at( x[, ...indices] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/at]</span><span class="delimiter">: </span><span class="description">return an `ndarray` element.</span>
-   <span class="signature">[`broadcastArray( x, shape )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/broadcast-array]</span><span class="delimiter">: </span><span class="description">broadcast an ndarray to a specified shape.</span>
-   <span class="signature">[`broadcastArrays( ...arrays )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/broadcast-arrays]</span><span class="delimiter">: </span><span class="description">broadcast ndarrays to a common shape.</span>
-   <span class="signature">[`castingModes()`][@devtea2026/temporibus-assumenda-explicabo-ipsa/casting-modes]</span><span class="delimiter">: </span><span class="description">list of ndarray casting modes.</span>
-   <span class="signature">[`dataBuffer( x )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/data-buffer]</span><span class="delimiter">: </span><span class="description">return the underlying data buffer of a provided ndarray.</span>
-   <span class="signature">[`defaults()`][@devtea2026/temporibus-assumenda-explicabo-ipsa/defaults]</span><span class="delimiter">: </span><span class="description">default ndarray settings.</span>
-   <span class="signature">[`dispatch( fcns, types, data, nargs, nin, nout )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/dispatch]</span><span class="delimiter">: </span><span class="description">create an ndarray function interface which performs multiple dispatch.</span>
-   <span class="signature">[`dtype( x )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/dtype]</span><span class="delimiter">: </span><span class="description">return the data type of a provided ndarray.</span>
-   <span class="signature">[`dtypes( [kind] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/dtypes]</span><span class="delimiter">: </span><span class="description">list of ndarray data types.</span>
-   <span class="signature">[`emptyLike( x[, options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/empty-like]</span><span class="delimiter">: </span><span class="description">create an uninitialized ndarray having the same shape and data type as a provided ndarray.</span>
-   <span class="signature">[`empty( shape[, options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/empty]</span><span class="delimiter">: </span><span class="description">create an uninitialized ndarray having a specified shape and data type.</span>
-   <span class="signature">[`FancyArray( dtype, buffer, shape, strides, offset, order[, options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/fancy]</span><span class="delimiter">: </span><span class="description">fancy multidimensional array constructor.</span>
-   <span class="signature">[`flag( x, name )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/flag]</span><span class="delimiter">: </span><span class="description">return a specified flag for a provided ndarray.</span>
-   <span class="signature">[`flags( x )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/flags]</span><span class="delimiter">: </span><span class="description">return the flags of a provided ndarray.</span>
-   <span class="signature">[`scalar2ndarray( value[, options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/from-scalar]</span><span class="delimiter">: </span><span class="description">convert a scalar value to a zero-dimensional ndarray.</span>
-   <span class="signature">[`ind2sub( shape, idx[, options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/ind2sub]</span><span class="delimiter">: </span><span class="description">convert a linear index to an array of subscripts.</span>
-   <span class="signature">[`indexModes()`][@devtea2026/temporibus-assumenda-explicabo-ipsa/index-modes]</span><span class="delimiter">: </span><span class="description">list of ndarray index modes.</span>
-   <span class="signature">[`maybeBroadcastArray( x, shape )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/maybe-broadcast-array]</span><span class="delimiter">: </span><span class="description">broadcast an ndarray to a specified shape if and only if the specified shape differs from the provided ndarray's shape.</span>
-   <span class="signature">[`maybeBroadcastArrays( arrays )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/maybe-broadcast-arrays]</span><span class="delimiter">: </span><span class="description">broadcast ndarrays to a common shape.</span>
-   <span class="signature">[`minDataType( value )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/min-dtype]</span><span class="delimiter">: </span><span class="description">determine the minimum ndarray data type of the closest "kind" necessary for storing a provided scalar value.</span>
-   <span class="signature">[`mostlySafeCasts( [dtype] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/mostly-safe-casts]</span><span class="delimiter">: </span><span class="description">return a list of ndarray data types to which a provided ndarray data type can be safely cast and, for floating-point data types, can be downcast.</span>
-   <span class="signature">[`ndims( x )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/ndims]</span><span class="delimiter">: </span><span class="description">return the number of ndarray dimensions.</span>
-   <span class="signature">[`nextDataType( [dtype] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/next-dtype]</span><span class="delimiter">: </span><span class="description">return the next larger ndarray data type of the same kind.</span>
-   <span class="signature">[`numelDimension( x, dim )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/numel-dimension]</span><span class="delimiter">: </span><span class="description">return the size (i.e., number of elements) of a specified dimension for a provided ndarray.</span>
-   <span class="signature">[`numel( x )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/numel]</span><span class="delimiter">: </span><span class="description">return the number of elements in an ndarray.</span>
-   <span class="signature">[`offset( x )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/offset]</span><span class="delimiter">: </span><span class="description">return the index offset specifying the underlying buffer index of the first iterated ndarray element.</span>
-   <span class="signature">[`order( x )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/order]</span><span class="delimiter">: </span><span class="description">return the layout order of a provided ndarray.</span>
-   <span class="signature">[`orders()`][@devtea2026/temporibus-assumenda-explicabo-ipsa/orders]</span><span class="delimiter">: </span><span class="description">list of ndarray orders.</span>
-   <span class="signature">[`outputDataTypePolicies()`][@devtea2026/temporibus-assumenda-explicabo-ipsa/output-dtype-policies]</span><span class="delimiter">: </span><span class="description">list of output ndarray data type policies.</span>
-   <span class="signature">[`promotionRules( [dtype1, dtype2] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/promotion-rules]</span><span class="delimiter">: </span><span class="description">return the ndarray data type with the smallest size and closest "kind" to which ndarray data types can be **safely** cast.</span>
-   <span class="signature">[`safeCasts( [dtype] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/safe-casts]</span><span class="delimiter">: </span><span class="description">return a list of ndarray data types to which a provided ndarray data type can be safely cast.</span>
-   <span class="signature">[`sameKindCasts( [dtype] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/same-kind-casts]</span><span class="delimiter">: </span><span class="description">return a list of ndarray data types to which a provided ndarray data type can be safely cast or cast within the same "kind".</span>
-   <span class="signature">[`shape( x )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/shape]</span><span class="delimiter">: </span><span class="description">return the shape of a provided ndarray.</span>
-   <span class="signature">[`sliceAssign( x, y, ...s[, options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/slice-assign]</span><span class="delimiter">: </span><span class="description">assign element values from a broadcasted input `ndarray` to corresponding elements in an output `ndarray` view.</span>
-   <span class="signature">[`sliceDimensionFrom( x, dim, start[, options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/slice-dimension-from]</span><span class="delimiter">: </span><span class="description">return a read-only shifted view of an input `ndarray` along a specified dimension.</span>
-   <span class="signature">[`sliceDimensionTo( x, dim, stop[, options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/slice-dimension-to]</span><span class="delimiter">: </span><span class="description">return a read-only truncated view of an input `ndarray` along a specified dimension.</span>
-   <span class="signature">[`sliceDimension( x, dim, slice[, options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/slice-dimension]</span><span class="delimiter">: </span><span class="description">return a read-only view of an input `ndarray` when sliced along a specified dimension.</span>
-   <span class="signature">[`sliceFrom( x, ...start[, options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/slice-from]</span><span class="delimiter">: </span><span class="description">return a read-only shifted view of an input ndarray.</span>
-   <span class="signature">[`sliceTo( x, ...stop[, options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/slice-to]</span><span class="delimiter">: </span><span class="description">return a read-only truncated view of an input ndarray.</span>
-   <span class="signature">[`slice( x, ...s[, options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/slice]</span><span class="delimiter">: </span><span class="description">return a read-only view of an input `ndarray`.</span>
-   <span class="signature">[`stride( x, dim )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/stride]</span><span class="delimiter">: </span><span class="description">return the stride along a specified dimension for a provided ndarray.</span>
-   <span class="signature">[`strides( x )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/strides]</span><span class="delimiter">: </span><span class="description">return the strides of a provided ndarray.</span>
-   <span class="signature">[`sub2ind( shape, ...subscripts[, options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/sub2ind]</span><span class="delimiter">: </span><span class="description">convert subscripts to a linear index.</span>
-   <span class="signature">[`ndarray2array( x )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/to-array]</span><span class="delimiter">: </span><span class="description">convert an ndarray to a generic array.</span>
-   <span class="signature">[`zerosLike( x[, options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/zeros-like]</span><span class="delimiter">: </span><span class="description">create a zero-filled ndarray having the same shape and data type as a provided ndarray.</span>
-   <span class="signature">[`zeros( shape[, options] )`][@devtea2026/temporibus-assumenda-explicabo-ipsa/zeros]</span><span class="delimiter">: </span><span class="description">create a zero-filled ndarray having a specified shape and data type.</span>

</div>

<!-- </toc> -->

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- TODO: better examples -->

<!-- eslint no-undef: "error" -->

```javascript
var objectKeys = require( '@stdlib/utils/keys' );
var ns = require( '@devtea2026/temporibus-assumenda-explicabo-ipsa' );

console.log( objectKeys( ns ) );
```

</section>

<!-- /.examples -->

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

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@devtea2026/temporibus-assumenda-explicabo-ipsa.svg
[npm-url]: https://npmjs.org/package/@devtea2026/temporibus-assumenda-explicabo-ipsa

[test-image]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/devtea2026/temporibus-assumenda-explicabo-ipsa/main.svg
[coverage-url]: https://codecov.io/github/devtea2026/temporibus-assumenda-explicabo-ipsa?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/devtea2026/temporibus-assumenda-explicabo-ipsa.svg
[dependencies-url]: https://david-dm.org/devtea2026/temporibus-assumenda-explicabo-ipsa/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/deno
[deno-readme]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/blob/deno/README.md
[umd-url]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/umd
[umd-readme]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/blob/umd/README.md
[esm-url]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/esm
[esm-readme]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/blob/esm/README.md
[branches-url]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/devtea2026/temporibus-assumenda-explicabo-ipsa/main/LICENSE

<!-- <toc-links> -->

[@devtea2026/temporibus-assumenda-explicabo-ipsa/at]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/at

[@devtea2026/temporibus-assumenda-explicabo-ipsa/broadcast-array]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/broadcast-array

[@devtea2026/temporibus-assumenda-explicabo-ipsa/broadcast-arrays]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/broadcast-arrays

[@devtea2026/temporibus-assumenda-explicabo-ipsa/casting-modes]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/casting-modes

[@devtea2026/temporibus-assumenda-explicabo-ipsa/data-buffer]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/data-buffer

[@devtea2026/temporibus-assumenda-explicabo-ipsa/defaults]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/defaults

[@devtea2026/temporibus-assumenda-explicabo-ipsa/dispatch]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/dispatch

[@devtea2026/temporibus-assumenda-explicabo-ipsa/dtype]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/dtype

[@devtea2026/temporibus-assumenda-explicabo-ipsa/dtypes]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/dtypes

[@devtea2026/temporibus-assumenda-explicabo-ipsa/empty-like]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/empty-like

[@devtea2026/temporibus-assumenda-explicabo-ipsa/empty]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/empty

[@devtea2026/temporibus-assumenda-explicabo-ipsa/fancy]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/fancy

[@devtea2026/temporibus-assumenda-explicabo-ipsa/flag]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/flag

[@devtea2026/temporibus-assumenda-explicabo-ipsa/flags]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/flags

[@devtea2026/temporibus-assumenda-explicabo-ipsa/from-scalar]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/from-scalar

[@devtea2026/temporibus-assumenda-explicabo-ipsa/ind2sub]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/ind2sub

[@devtea2026/temporibus-assumenda-explicabo-ipsa/index-modes]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/index-modes

[@devtea2026/temporibus-assumenda-explicabo-ipsa/maybe-broadcast-array]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/maybe-broadcast-array

[@devtea2026/temporibus-assumenda-explicabo-ipsa/maybe-broadcast-arrays]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/maybe-broadcast-arrays

[@devtea2026/temporibus-assumenda-explicabo-ipsa/min-dtype]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/min-dtype

[@devtea2026/temporibus-assumenda-explicabo-ipsa/mostly-safe-casts]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/mostly-safe-casts

[@devtea2026/temporibus-assumenda-explicabo-ipsa/ndims]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/ndims

[@devtea2026/temporibus-assumenda-explicabo-ipsa/next-dtype]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/next-dtype

[@devtea2026/temporibus-assumenda-explicabo-ipsa/numel-dimension]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/numel-dimension

[@devtea2026/temporibus-assumenda-explicabo-ipsa/numel]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/numel

[@devtea2026/temporibus-assumenda-explicabo-ipsa/offset]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/offset

[@devtea2026/temporibus-assumenda-explicabo-ipsa/order]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/order

[@devtea2026/temporibus-assumenda-explicabo-ipsa/orders]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/orders

[@devtea2026/temporibus-assumenda-explicabo-ipsa/output-dtype-policies]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/output-dtype-policies

[@devtea2026/temporibus-assumenda-explicabo-ipsa/promotion-rules]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/promotion-rules

[@devtea2026/temporibus-assumenda-explicabo-ipsa/safe-casts]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/safe-casts

[@devtea2026/temporibus-assumenda-explicabo-ipsa/same-kind-casts]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/same-kind-casts

[@devtea2026/temporibus-assumenda-explicabo-ipsa/shape]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/shape

[@devtea2026/temporibus-assumenda-explicabo-ipsa/slice-assign]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/slice-assign

[@devtea2026/temporibus-assumenda-explicabo-ipsa/slice-dimension-from]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/slice-dimension-from

[@devtea2026/temporibus-assumenda-explicabo-ipsa/slice-dimension-to]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/slice-dimension-to

[@devtea2026/temporibus-assumenda-explicabo-ipsa/slice-dimension]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/slice-dimension

[@devtea2026/temporibus-assumenda-explicabo-ipsa/slice-from]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/slice-from

[@devtea2026/temporibus-assumenda-explicabo-ipsa/slice-to]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/slice-to

[@devtea2026/temporibus-assumenda-explicabo-ipsa/slice]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/slice

[@devtea2026/temporibus-assumenda-explicabo-ipsa/stride]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/stride

[@devtea2026/temporibus-assumenda-explicabo-ipsa/strides]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/strides

[@devtea2026/temporibus-assumenda-explicabo-ipsa/sub2ind]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/sub2ind

[@devtea2026/temporibus-assumenda-explicabo-ipsa/to-array]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/to-array

[@devtea2026/temporibus-assumenda-explicabo-ipsa/zeros-like]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/zeros-like

[@devtea2026/temporibus-assumenda-explicabo-ipsa/zeros]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/zeros

[@devtea2026/temporibus-assumenda-explicabo-ipsa/base]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/base

[@devtea2026/temporibus-assumenda-explicabo-ipsa/iter]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/iter

[@devtea2026/temporibus-assumenda-explicabo-ipsa/array]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/array

[@devtea2026/temporibus-assumenda-explicabo-ipsa/ctor]: https://github.com/devtea2026/temporibus-assumenda-explicabo-ipsa/tree/main/ctor

<!-- </toc-links> -->

</section>

<!-- /.links -->
