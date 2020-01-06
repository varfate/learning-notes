# JavaScript类型-细节

## 7 种基本类型

1. `Undefined`
2. `Null`
3. `Boolean`
4. `String`
5. `Number`
6. `Symbol`
7. `Object`

## Undefined VS Null

### Undefined

1. 意义: 未定义

2. 非关键字
> [MDN 关于Undefined的描述](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined)

- 由于可以被重新赋值,所以 `undefined` 的值并不一定为 `undefined`
- eg:
```javascript
(function() {
  // 此处不会报错
  var undefined = 'foo';
  console.log(undefined, typeof undefined);
})();
```
- 以上就解释了 void 0 代替 undefined 的原因

### Null

1. 意义: 定义了, 但是值为空
2. 是关键字

```javascript
var null = 1 // 会报错
// Uncaught SyntaxError: Unexpected token 'null'
```
