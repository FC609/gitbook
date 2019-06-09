# book.json配置

新建一个`book.json`文件，可以用来配置gitbook。

## title 

设置书本的标题

```JSON
 "title": "个人笔记"
```

## author

作者的相关信息

```JSON
 "author": "fc"
```

## description

简单描述

```JSON
"descirption": "记录一些个人比较感兴趣的小东西"
```

## language

Gitbook使用的语言

```JSON
"language" : "zh-hans"
```
> en, ar, bn, cs, de, en, es, fa, fi, fr, he, it, ja, ko, no, pl, pt, ro, ru, sv, uk, vi, zh-hans, zh-tw

## styles 

自定义页面样式
默认情况下各generator对应的css文件

```JSON
"styles": {
    "website": "styles/website.css",
    "ebook": "styles/ebook.css",
    "pdf": "styles/pdf.css",
    "mobi": "styles/mobi.css",
    "epub": "styles/epub.css"
}
```

## links

在左侧导航栏添加链接信息

```JSON
"links" : {
    "sidebar" : {
        "Personal Book" : "http://www.gtwteam.com"
    }
}
```

## 插件

可以在插件前面加-符号删除默认插件，默认五种插件如下
- highlight：代码高亮
- search：导航栏查询功能（不支持中文）
- sharing：右上角分享功能
- font-settings：字体设置（最上方的"A"符号）
- livereload：为GitBook实时重新加载

> 更多插件链接

- <https://github.com/zhangjikai/gitbook-use/blob/master/plugins.md>
- <https://github.com/zq99299/gitbook-plugin-anchor-navigation-ex/blob/master/doc/config.md>
- <https://github.com/crifan/gitbook_template>
- <https://www.cnblogs.com/zhangjk1993/p/5066771.html>


> 感恩的心，感谢各位
> jsliang的掘金： <https://juejin.im/post/5ce51e126fb9a07ed440d7d0>
> jsliang的github： <https://liangjunrong.github.io/>