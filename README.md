<div align="center">

<br>

<h1>modern-grid</h1>

[![npm](https://img.shields.io/npm/v/modern-grid.svg?colorB=brightgreen)](https://www.npmjs.com/package/modern-grid)
[![GitHub package version](https://img.shields.io/github/package-json/v/ux-ui-pro/modern-grid.svg)](https://github.com/ux-ui-pro/modern-grid)
[![NPM Downloads](https://img.shields.io/npm/dm/modern-grid.svg?style=flat)](https://www.npmjs.org/package/modern-grid)

<sup><a href="https://bundlephobia.com/package/modern-grid">370 bytes gzipped</a></sup>
<h3><a href="https://ux-ui-pro.github.io/modern-grid/dist/">Demo</a></h3>

</div>
<br>

### Import
<sub>Import file if your bundler supports SCSS.</sub>
```SCSS
@import "node_modules/modern-grid/src/modern-grid.scss";
```
```SCSS
@import url("/node_modules/modern-grid/src/modern-grid.scss") screen and (min-width: 992px);
```
<sub>Or link to the file by the `<link>` element:</sub>
```HTML
<link rel="stylesheet" href="path-to-the-file/modern-grid.min.css">
```
<br>

### Usage
```CSS
:root {
    --wrapper: min(1600px, 92vw);
    --gutter: 3vw;
}
```
```HTML
<div class="wrapper">
	<div class="column" style="--column: 2; --offset: 2;">column 2 offset 2</div>
	<div class="column" style="--column: 5;">column 5</div>
	<div class="column column--infinite" style="--column: 3;">column 3 infinite</div>
</div>
```
<br>

### Settings

| Class&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Description |
| --- | --- |
| `.wrapper` | ... |
| `.column` | ... |
| `.column--infinite` | Stretches the first or last column to the edge of the screen. |
<br>

| Variable&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Description |
| --- | --- |
| `--wrapper` | Sets the width of the wrapper and the size of the margins from the wrapper on the left and right. For example: `80vw` or `calc(100vw - 100px)` or `min(1600px, 92vw)`. |
| `--gutter` | Sets the size of the margins between the columns. |
| `--column` | Used to set the width of one column. Allowed to use positive decimals. Example: `--column: 3.5`. |
| `--offset` | Move columns to the right using `--offset` variables. These variables increase the left margin of a column. For example, `--column: 8; --offset: 4;`. |
<br>

### License
<sub>modern-grid is released under MIT license.</sub>