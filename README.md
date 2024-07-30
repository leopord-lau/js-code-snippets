# js-code-snippets
<div align="center">
  <img width="340" alt="performance and build size charts" src="./images/code-snippets.jpg">
</div>
本仓库收集了包含各种各样的 ES6 辅助函数代码段，包含了用于处理不同 js 类型、数据结构、算法、dom 操作，Math 运算以及 node 相关方法，用于帮助大家在碎片时间快速学习、记忆一些 js 相关内容。

## string 相关

### js 中的字符串都是不可变的

不同程语言之间的字符串规范各不相同，但大多数语言都将其视为引用类型。但是 JavaScript 中的字符串与他们不同，它们是不可变的原始值。这意味着其中的**字符不会改变，对字符串的任何操作实际上都会创建新的字符串**。

```js
const str = 'string';
str[1] = 'a';          // 没有任何作用，也不会报错
console.log(str)       // 'string'
```

如果我们想更好地理解字符串是如何工作的，那么我们可以把字符串看成是数字（Number 类型）。数字也是不可变的原始类型。例如，如果我们想改变数字，我们可以将一个数值（比如 11）更改为另一个数字（比如 12）。那么字符串也类似，我们不能改变字符串（比如 `string` ）中其中一个字符（比如 `t`）来使其成为另一个字符串（比如 `saring`）。
