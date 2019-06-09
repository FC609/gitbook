# gitbook


> 使用gitBook 首先 是会markdown语法和node中npm下载包



- 安装

```
npm i -g gitbook-cli
```

- 初始化

```
gitbook init
```
会自动生成两个必要的文件 `README.md` 和 `SUMMARY.md`。

- 预览

```
gitbook serve 
```
gitbook会启动一个4000端口用于预览，可以在浏览器打开网址：` http://localhost:4000 `预览效果。

- 查看版本

```
gitbook -V
```

- 更新到gitbook的最新版本

```
gitbook update 
```

- 帮助文档

```
gitbook --help
```

- 生成静态网页

```
gitbook build
```

- 生成静态网页时指定gitbook的版本，如果本地没有将先下载

```
gitbook build --gitbook=3.2.3
```

- 列出所有的gitbook版本

```
gitbook ls
```

- 列出远程可用的gitbook版本

```
gitbook ls-remote
```

- 卸载对应的gitbook版本

```
gitbook uninstall 3.2.3
```

- 安装依赖

```
gitbook install
```

- 指定log的级别

```
gitbook build --log=debug
```

- 输出错误信息

```
gitbook builid --debug
```

> 感恩的心，感谢大佬的探索
> 大佬的gitbook：<http://www.lijiam.com/part2/gitbook/>
