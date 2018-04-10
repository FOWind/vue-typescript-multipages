# Vue多页+Typescript模板

## 介绍

参考资料

[vue-typescript-start](https://github.com/ws456999/vue-typescript-starter)

[用vue构建多页面应用](https://segmentfault.com/a/1190000011265006)

按照[vue-typescript-start](https://github.com/ws456999/vue-typescript-starter)引入TyperScript的话会报错：`Module build failed: TypeError: Cannot read property 'afterCompile' of undefined`，主要原因是：默认安装的ts-loader为4.x版，版本不兼容。解决方法是将使用命令
``` bash
npm uninstall ts-loader
```
将原来的ts-loader卸载，然后使用命令
```npm
npm install --save ts-loader@3.x
```
安装ts-loader3.x版


> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# run unit tests
npm run unit

# run e2e tests
npm run e2e

# run all tests
npm test
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
