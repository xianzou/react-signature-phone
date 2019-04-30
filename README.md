[![npm package](https://img.shields.io/badge/npm-0.0.6-orange.svg?style=flat-square)](https://www.npmjs.com/package/react-signature-pad)



# React Signature phone
### forked 项目 react-signature-pad

- react版本的移动端电子签名
- 修改源码去除canvas缩放,自适应手机宽度
- 添加自定义 height（默认值200） 和width (默认值window.innerWidth)
- 原项目地址[react-signature-pad](https://github.com/blackjk3/react-signature-pad)

## 安装

```bash
$ yarn add react-signature-phone
or
$ npm install react-signature-phone
```



# 使用方式

```javascript
import React from 'react';
import SignaturePad from 'react-signature-pad';

React.render(
  <SignaturePad clearButton="true" width={300} height={150} />,
  document.body
)
```

# 方法

```javascript
<SignaturePad clearButton="true" ref="mySignature" />
...

var signature = this.refs.mySignature;

// Methods

// ===============================================
// isEmpty() - returns boolean
// ===============================================

signature.isEmpty();

// ===============================================
// clear() - clears canvas
// ===============================================

signature.clear();

// ===============================================
// toDataURL() - 将canvas转化成base64图
// ===============================================

signature.toDataURL();

// ===============================================
// fromDataURL() - 将base64图写入canvas
// ===============================================

signature.fromDataURL(base64String);

```

# CSS
一般不需要样式，如果需要样式点击这里： [this file](style.css),

# Example
```bash
$ yarn start
```
打开浏览器访问http://localhost:8080/ 
