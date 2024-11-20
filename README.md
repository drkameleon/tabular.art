
<p align="center"><img align="center" width="350" src="https://raw.githubusercontent.com/drkameleon/tabular.art/main/logo.png"/></p>
<p align="center">
  <b>Feature-rich ASCII table generator<br>for Arturo</b>
  <br><br>
  <img src="https://img.shields.io/github/license/arturo-lang/grafito?style=for-the-badge">
  <img src="https://img.shields.io/badge/language-Arturo-orange.svg?style=for-the-badge">

</p>

--- 
 
<!--ts-->

* [What does this package do?](#what-does-this-package-do)
* [How do I use it?](#how-do-i-use-it)
* [Function Reference](#function-reference)
* [License](#license)   

<!--te-->
 
---

### What does this package do?

This package includes a simple - but powerful - ASCII table generator

### How do I use it?

Simply `import` it and use any of the provided helper functions:

```red
import "tabular"!

print toTable [
    ["1.1" "2.1" "3.1"]
    ["1.2" "2.2" "3.2"]
]
```

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
