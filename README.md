
# pangu

盘古之白。中文自动规范化工具。

## Install

via npm:

```
$ npm install hundun [-g]
```

## Usage

### CLI

```
$ pangu file.md
$ pangu ./dir
$ pangulint file.md
```

### NodeJS

```js
var pangu = require('hundun');
pangu(text);
pangu.markdown(markdown);
```

## API

### pangu(text, options)

自动规范化修复文本格式。

### pangu.fixup(text, options)

同 `pangu(text, options)`。

### pangu.lint(markdown options)

校验文档。

## Options

* file_type: 目前支持 `[text, markdown]`，默认为 `text`。
* trailling_whitespace: 允许行尾空白字符。默认为 `true`，如果设置为 `false`，则剔除行尾空白。
* pangu_spacing: 盘古之白，中英文之间的空白。默认为 `" "`，你也可以设置为 `""` 或双宽度空白 `"TODO"`。