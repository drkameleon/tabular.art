
<p align="center"><img align="center" width="350" src="https://raw.githubusercontent.com/drkameleon/tabular.art/main/logo.png"/></p>
<p align="center">
  <b>Feature-rich ASCII table generator<br>for Arturo</b>
  <br><br>
  <img src="https://img.shields.io/github/license/arturo-lang/grafito?style=for-the-badge">
  <img src="https://img.shields.io/badge/language-Arturo-orange.svg?style=for-the-badge">

</p>

<p align="center"><img width="90%" align="center" src="https://raw.githubusercontent.com/drkameleon/tabular.art/main/screenshot.png"/></p>

--- 
 
<!--ts-->

* [What does this package do?](#what-does-this-package-do)
* [How do I use it?](#how-do-i-use-it)
* [Function Reference](#function-reference)
* [License](#license)   

<!--te-->
 
---

### What does this package do?

This package includes a simple - but powerful - ASCII table generator, with all the (tabular) [bells](https://www.youtube.com/watch?v=BfWJqKIxyGc) and whistles, bundled in an easy-to-use package for Arturo.

### How do I use it?

Simply `import` it and use any of the provided helper functions; mainly, one: `tabular`.

> [!TIP]
> The code below generates the exact same tables 
> you may see in the screenshot above^ :wink:

```red
import "tabular"!

; A simple table
print tabular [
    [1 2 3]
    [4 5 6]
]

; A table with header
print tabular.header:["Item" "Qty" "Price"][
    ["Apples"    5   2.99]
    ["Oranges"   10  3.49]
    ["Bananas"   8   1.99]
]

; A table with header and custom-aligned columns
print tabular
    .header:["Item" "Qty" "Price"] 
    .align:['left 'right 'right]
[
    ["Apples"  5  2.99]
    ["Oranges" 10 3.49]
    ["Bananas" 8  1.99]
]

; A Unicode-based table with custom-aligned columns
; and variable, user-defined paddings
print tabular.unicode
    .padding:[1 4 2]
    .align:['left 'center 'right] 
[
    ["narrow" "widest" "mid"]
    ["col1"   "col2"   "col3"]
]
```

### Function reference

#### `tabular`

##### Description

Create a new ASCII table with given rows

##### Usage

<pre>
<b>tabular</b> <ins>rows</ins> <i>:block</i>
</pre>

##### Attributes

| Option | Type(s) | Description |
|----|----|----|
| header | :block | set table header columns |
| align | :literal, :block | set column alignments (single value or array) |
| unicode | :logical | use Unicode characters |
| padding | :integer, :block | set custom padding per column (single value or array) |

##### Returns

- *:string*

<hr/>

### License

MIT License

Copyright (c) 2024 Yanis Zafirópulos

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
