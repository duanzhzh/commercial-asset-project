# redux+sagas项目设计


## 说明
***本项目是为较为复杂的前端项目搭的框架，借助Redux进行数据和组件的状态的管理，基于redux-sagas中间件进行Redux Action部分的异步操作管理。***

## 功能描述
- [x] 交易频道
- [x] 资讯频道
- [x] 榜单频道
- [x] 个人中心
- [详情见WIKI](https://github.com/duanzhzh/commercial-asset-project/wiki/%E9%A1%B9%E7%9B%AE%E6%A8%A1%E5%9D%97%E5%88%86%E8%A7%A3)

## 技术栈
- [x] react
- [x] react-router-dom
- [x] react-redux
- [x] redux-saga
- [x] fetch
- [x] webpack
- [x] antd-design-mobile
- [x] echart
- [x] react-bmap

## 项目目录
- [x] build -- 存放编译后的静态文件
- [x] config -- webpack相关的配置
- [x] public -- 存放模板文件
- [x] script  -- node 执行脚本
- [x] src -- 项目相关的文件
  - [x] components -- 共用子组件
  - [x] containers -- 组件
  - [x] fetch -- 网络请求
  - [x] reducers -- store data 模块
  - [x] sagas -- reducers异步操作模块
  - [x] scss -- 共用样式
  - [x] App.js -- route manage 、public modules import
  - [x] index.js -- 项目入口文件
- [x] package.json -- 项目配置文件
- [x] README.md -- 项目说明

## Todo
- 根据设计稿设计和api定Redux数据结构……
- 根据设计稿开发UI……

## 代码规范
- 项目代码语法采用ES6+ES7标准；
- 项目代码风格规范严格遵守 [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html)

## 打包
为了便于部分页面可能使用在APP上和小程序上
- 按照路由层级进行代码分割打包
- 引用包打包成public chrunk

## 运行环境
node v8.4.0

## 发布
打包发布静态项目，启动脚本在根目录下执行
- 生产环境运行：npm run build 
- 预发布环境运行：npm run build:pre 
- 测试环境运行：npm run build:dev <br>

打包好的代码在build目录下


