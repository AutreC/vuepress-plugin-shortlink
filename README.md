# [vuepress-plugin-shortlink](https://iout.io/open/vuepress-plugin-shortlink)

A vuepress plugin for generate static post link based on post file name.

## 安装

```
npm install vuepress-plugin-shortlink --save
```

从config.js配置中删除 permalink，该插件是基于默认永久链接/:regular


## 例子

### version 1.0
```
source: /books/a-book.md
permalink: /books/261f97f7.html

source: /hello-word.md
permalink: /b1d4025b.html

source: /books/computer/a-book.md
permalink: /books/computer/261f97f7.html
```

## 设定参数

该插件基于vuepress-plugin-clean-urls，可以自定义后缀和404，设定方法同vuepress-plugin-clean-urls

```
plugins: [
    [
      'vuepress-plugin-shortlink',
      {
        normalSuffix: '/',
        indexSuffix: '/',
        notFoundPath: '/404.html',
      },
    ],
  ],
```


## ThanksFor

[vuepress-plugin-clean-urls](https://github.com/vuepress/vuepress-plugin-clean-urls) [sheetjs](https://github.com/SheetJS/js-crc32)
