#### 屏蔽内容可编辑的警告
```jsx
<div suppressContentEditableWarning={true} contentEditable={true}></div>
```

`suppressContentEditableWarning = true` 用来屏蔽内容可编辑的警告。

#### 获取div的offsetTop位置

```javascript
import ReactDOM from 'react-dom';
//...
componentDidMount() {
    var rect = ReactDOM.findDOMNode(this).getBoundingClientRect()
}
```

