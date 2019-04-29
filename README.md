[![npm package](https://img.shields.io/badge/npm-0.0.6-orange.svg?style=flat-square)](https://www.npmjs.com/package/react-signature-pad)



# React Signature Pad
### forked 项目 react-signature-pad，修改源码去除canvas缩放,自适应手机宽度,添加自定义 height（默认值200） 和width (默认值window.innerWidth)
A [signature pad](https://github.com/xianzou/react-signature-phone) implementation for react.
B 原项目地址[react-signature-pad](https://github.com/blackjk3/react-signature-pad)

# Basic Usage

```javascript
var React = require('react');
var SignaturePad = require('react-signature-pad');

React.render(
  <SignaturePad clearButton="true" width={300} height={150} />,
  document.body
)
```

# Methods

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
// toDataURL() - retrieves image as a data url
// ===============================================

signature.toDataURL();

// ===============================================
// fromDataURL() - writes a base64 image to canvas
// ===============================================

signature.fromDataURL(base64String);

```

# CSS
In order to make the signature pad work correctly you will need the css as well.  All the relevant styles are in [this file](style.css).

# Example
```bash
$ npm start
```
Then navigate to http://localhost:8080/ in your browser and you should be able to see the signature pad in action.
