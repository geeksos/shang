
### 快速搭建开发 san helloworld

npm init -y 新建 package.json

```
npm install --save san
npm install --save preact
npm install --save preact-compat
npm install --save-dev parcel-bundler
npm install --save-dev babel-preset-env
npm install --save-dev babel-preset-preact
```

然后确保以下 Babel 预设存在.

```js
// .babelrc
{
  "presets": ["env", "preact"]
}
```

添加 start 指令到 package.json

```js
// package.json
"scripts": {
  "start": "parcel index.html"
}
```

运行

```js
npm start
```

* * *

1. 了解最新的 parcel

2. 使用webpack4或parcel搭建一个开发环境

   ​

任务要求：

- 支持js、css格式的解析

- 区分 development / production 环境

- 使用npm scripts设罝dev、test、build命令

- 写一个san组件并在浏览器中显示hello world

- 使用babel-loader进行js代码转换

  ​

参考资料

- <https://github.com/baidu/san>
- [https://webpack.js.org](https://webpack.js.org/)
- <https://medium.com/webpack>
- <https://parceljs.org/>