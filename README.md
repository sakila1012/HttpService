# HttpService
封装 axios

在网上搜了好多关于 axios 的封装，发现他们均无法使用，通用型不太好。所以自己就动手封装了一个适用的组件，该组件封装了常用的 get，post，put，delete请求。

## 第一步 安装 axios，iview

引入 iview 主要是对异步交互过程中一种友好的用户体验，让用户能够体验到页面不是没有反应，而是在等待服务器的响应。

## 第二步 创建 HttpService.js

在 src > api 目录下 创建 HttpService.js，具体内容见下

## 第三步 在main.js，引入 HttpService.js

## 第四步， 在任意组件中使用

引用示例：

get 请求
```
this.$api.get("/api/v1/...", data).then(response => {
  console.log(response)
})
```

post 请求
```
this.$api.post("/api/v1/...", data).then(response => {
  console.log(response)
})
```
错误之处，欢迎指正。
