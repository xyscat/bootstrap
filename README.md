# Bootstrap 3 起步

简要介绍，如何下载、使用、基本模板和案例……

[Bootstrap博客](http://blog.getbootstrap.com/)

目录：

- 使用
- 包含内容
- 基本模板
- Bootlint
- 禁止响应式布局

## 使用

用于生产环境的 Bootstrap：编译并压缩后的CSS、JS、字体文件。不含文档和源码文件。

CDN 服务：

```
<!-- 新 Bootstrap 核心 CSS 文件 -->
<link rel="stylesheet" href="http://cdn.bootcss.com/bootstrap/3.3.0/css/bootstrap.min.css">

<!-- 可选的Bootstrap主题文件（一般不用引入） -->
<link rel="stylesheet" href="http://cdn.bootcss.com/bootstrap/3.3.0/css/bootstrap-theme.min.css">

<!-- jQuery文件。务必在bootstrap.min.js 之前引入 -->
<script src="http://cdn.bootcss.com/jquery/1.11.1/jquery.min.js"></script>

<!-- 最新的 Bootstrap 核心 JavaScript 文件 -->
<script src="http://cdn.bootcss.com/bootstrap/3.3.0/js/bootstrap.min.js"></script>
```
## 包含内容

目录结构：

```
bootstrap/
├── css/
│   ├── bootstrap.css
│   ├── bootstrap.min.css
│   ├── bootstrap-theme.css
│   └── bootstrap-theme.min.css
├── js/
│   ├── bootstrap.js
│   └── bootstrap.min.js
└── fonts/
    ├── glyphicons-halflings-regular.eot
    ├── glyphicons-halflings-regular.svg
    ├── glyphicons-halflings-regular.ttf
    └── glyphicons-halflings-regular.woff
```
## 基本模板

基本的HTML页面，文件的引入和使用。

实例精选：一些现成的页面实现，可以根据需要自己修改部分代码。

## Bootlint

[Bootstap](https://github.com/twbs/bootlint)的语法检测工具。

## 禁止响应式布局

Bootstrap它自动会进行响应式的适配，所以我们不需要去做响应式。

禁止响应式布局：

- 移除设置浏览器视口的viewport的meta标签。
- 为`.container`类设置一个`width`值覆盖框架默认的`width`设置，`width： 970px !important;`。
- 如何设置了导航条，需要移除所有导航条的折叠和展开行为。
- 对于栅格布局，额外增加`.col-xs-`类或替换掉`.col-md-`和`.col-lg-`。

> 所以说，在使用Bootstrap的时候就要避免响应式的设置。

> [Respond.js](https://github.com/scottjehl/Respond/blob/master/README.md#support--caveats)

> box-sizing属性
