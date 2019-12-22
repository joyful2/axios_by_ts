# ts-axios

使用 TypeScript 从零实现一个 axios

## Features

- 在浏览器端使用 XMLHttpRequest 对象通讯
- 支持 Promise API
- 支持请求和响应的拦截器
- 支持请求数据和响应数据的转换
- 支持请求的取消
- JSON 数据的自动转换
- 客户端防止 XSS

## Usage

```javascript
const axios = require('axios')

axios({
  method: 'post',
  url: '/user/12345',
  data: {
    firstName: 'Yee',
    lastName: 'Huang'
  }
})
```

<!-- test -->

类实现接口的时候，是实现的实例部分，而非构造器部分

构造器接口的使用：

类型保护：类型位词？， typeof,instance of, 自定义类型保护
extend 继承：本质上就是复制属性，且不覆盖原有属性
联合类型：|
交叉类型：&

如下这样调用函数时传参加：表示什么意思？表示值吗

!类型断言： Name! 表示告诉编译器 name 不为 null
Tsc test.ts —strictNullChecks

Request.onerror/ontimeout
继承内置对象时需要设置 Object.setPrototypeOf(this,SubClass.prototype)

导出类型文件：
Export \* from ./types

ts 使用思想： 1.先写实现再写接口 2.对外的实现才需要写接口，比如某些库不对外使用的 api 可以不用写接口，非公用的接口可以不抽离到 types.ts 文件

使用 markdown 记笔记，这样就能同步到 git，随时随地可以和线上同步
