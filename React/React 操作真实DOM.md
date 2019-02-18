# React 操作真实DOM

> 原文：[https://plainnany.github.io/2017/09/26/React-%E6%93%8D%E4%BD%9C%E7%9C%9F%E5%AE%9EDOM/](https://plainnany.github.io/2017/09/26/React-%E6%93%8D%E4%BD%9C%E7%9C%9F%E5%AE%9EDOM/)

最近在学习React的过程中遇到了一个问题，React怎么操作真实的DOM？

我们知道，React组件操作的DOM并不是真正的DOM，而是存在于内存之中的一种数据结构，叫做虚拟 DOM （virtual DOM）。只有当它插入文档以后，才会变成真实的 DOM 。根据 React 的设计，所有的 DOM 变动，都先在虚拟 DOM 上发生，然后再将实际发生变动的部分，反映在真实 DOM上，这种算法叫做 [DOM diff](https://calendar.perfplanet.com/2013/diff/) ，它可以极大提高网页的性能表现。但是在某些场景下，不得不操作真实的DOM，这个时候，就用到了`ref`这个属性。

假设有一个按钮，当用户点击的时候自动获取input文本框的焦点，用ref属性就可以实现。

html 代码

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>React demo</title>
  <!-- 引入react、react dom 的cdn文件  -->
  <script src="https://unpkg.com/react@15/dist/react.min.js"></script>
  <script src="https://unpkg.com/react-dom@15/dist/react-dom.min.js"></script>
</head>
<body>
  <div id="app"></div>
</body>
</html>
```

js代码（请选择JSX语法）

```javascript
var MyComponent = React.createClass({
  handleClick: function() {
    this.refs.myTextInput.focus()
  },
  render: function() {
    return (
      <div>
        <input type="text" ref="myTextInput" />
        <input type="button" value="click me" onClick={this.handleClick} />
      </div>
    )
  }
})
ReactDOM.render(
  <MyComponent />,
  document.getElementById('app')
)
```

在这个例子中，用户在input文本框中输入内容，这时必须获取真实的DOM节点，而在React中，虚拟的DOM是 拿不到用户的输入的，为了做到这一点，React提供了`ref`属性，然后 `this.refs.[refName]` 就会返回这个真实的 DOM 节点。对于上面的例子，就是 `this.refs.myTextInput`，通过给 `this.refs.myTextInput` 添加 `focus` 事件来获取input文本框的焦点。

需要注意的是，由于 `this.refs.myTextInput` 属性获取的是真实 DOM ，所以必须等到虚拟 DOM 插入文档以后，才能使用这个属性，否则会报错。上面代码中，通过为组件指定 Click 事件的回调函数，确保了只有等到真实 DOM 发生 Click 事件之后，才会读取 `this.refs.myTextInput` 属性。