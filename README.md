# format 

---
[![Build Status](https://travis-ci.org/dreamstu/format.svg?branch=master)](https://travis-ci.org/dreamstu/format)
[![spm version](http://spmjs.io/badge/format)](http://spmjs.io/package/format)

一套方便灵活的高可用的前端组合框架. 提供format格式化的基础组件

---

## Install

```
$ spm install format --save
```

## Usage

```js
var format = require('format');
// use format
```

---
## 方法概要

### format.date(format, formatString)

`释义`

让日期和时间按照指定的格式显示的方法

`参数`:

{String} format 格式字符串 

{String} formatString

`返回`:
{String} 返回生成的日期时间字符串

`示例`

````js
var d = new Date();
// 以 YYYY-MM-dd hh:mm:ss 格式输出 d 的时间字符串
format.date(d, "YYYY-MM-DD hh:mm:ss");
````


### format.number(num, pattern)

`释义`

让数字按照指定的格式显示的方法

`参数`

{String} num 要格式化的数字

{String} pattern 格式

`示例`

````js
format.number(12345.999,'#,##0.00');
 //out: 12,34,5.99
format.number(12345.999,'0'); 
 //out: 12345
format.number(1234.888,'#.0');
 //out: 1234.8
format.number(1234.888,'000000.000000');
 //out: 001234.888000
 ````