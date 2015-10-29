---
title: 安装
type: guide
order: 0
vue_version: 1.0.3
dev_size: "239.82"
min_size: "72.31"
gz_size: "23.73"
---

> **兼容性提示：** Vue.js 不支持 IE8 及其以下版本。

## 独立版本

直接下载并用 `<script>` 标签引入，`Vue` 被注册为一个全局变量。

<div id="downloads">
<a class="button" href="https://raw.github.com/vuejs/vue/{{vue_version}}/dist/vue.js" download>开发版本</a><span class="light info">包含丰富的注释和调试信息。</span>

<a class="button" href="https://raw.github.com/vuejs/vue/{{vue_version}}/dist/vue.min.js" download>生产版本</a><span class="light info">删除了警告，{{gz_size}}kb min+gzip</span>
</div>

### CDN

可以从 [jsdelivr](//cdn.jsdelivr.net/vue/{{vue_version}}/vue.min.js) 或 [cdnjs](//cdnjs.cloudflare.com/ajax/libs/vue/{{vue_version}}/vue.min.js) 获取（版本更新可能略滞后）。

### CSP 兼容版本

有些环境，如 Google Chrome Apps，强制应用内容安全策略 (CSP) ，不能使用 `new Function()` 对表达式求值。这时可以用 [CSP 兼容版本](https://github.com/vuejs/vue/tree/csp/dist)。

## NPM

在用 Vue.js 构建大型应用时推荐使用 NPM 安装，Vue.js 能很好地与 CommonJS 兼容模块打包器如 [Webpack](http://webpack.github.io/) 或 [Browserify](http://browserify.org/) 配合使用。Vue.js 也提供配套工具来开发[单文件组件](application.html#单文件组件)。

``` bash
# 最新稳定版本
$ npm install vue
# 最新稳定版本 + CSP 兼容版本
$ npm install vue@csp
# 开发版本（直接从 GitHub 安装）
$ npm install vuejs/vue#dev
```

## Bower

``` bash
# 最新稳定版本
$ bower install vue
```

## AMD 模块加载器

独立版本或通过 Bower 安装的版本已用 [UMD](https://github.com/umdjs/umd#readme) 包装，因此它们可以直接用作 AMD 模块。
