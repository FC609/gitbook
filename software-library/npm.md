[TOC]
# 有用的npm包

> npm i  -g  [module_name]

## npm -S -D -g 

**`npm install module_name -S: npm install module_name --save：`** 写入的dependencies 

**`npm install module_name -D: npm install module_name --save-dev：`** 写入devDependenices 

**`npm install module_name -g：`** 全局安装(命令行)

**`npm install module_name`** 本地安装(将安装包放在 ./node_modules 下)

## devDependencies和dependencies

- `devDependencies`用于本地环境开发时候。
- `dependencies` 用户发布环境

`devDependencies`是只会在开发环境下依赖的模块，生产环境不会被打入包内。通过`NODE_ENV=developement`或`NODE_ENV=production`指定开发还是生产环境。 
而`dependencies`依赖的包`不仅开发环境能使用，生产环境也能使用`。

## node管理
- nvm: <https://nvm.en.softonic.com/download>
- node: <https://nodejs.org/zh-cn/>
- nrm

## 编译
- nodemon
- typescript

## angular
- 脚手架: @angular/cli

## 样式
- less

## 工具
- gitbook-cli
- gulp
