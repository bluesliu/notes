# 在electron中实现跨域请求，无需更改服务器端设置

> 原文：[https://segmentfault.com/a/1190000012030202](https://segmentfault.com/a/1190000012030202)

很简单，在Electron的BrowserWindow模块中配置这样一个参数：

```javascript
mainWindow = new BrowserWindow({
	width: 800, 
	height: 600, 
	webPreferences: {webSecurity: false}
});
```

`webSecurity` 是什么意思呢？顾名思义，他是设置 web 安全性，如果参数设置为  `false`，它将禁用相同地方的规则 (通常测试服), 并且如果有2个非用户设置的参数，就设置 `allowDisplayingInsecureContent` 和 `allowRunningInsecureContent` 的值为 `true`。 （ `webSecurity` 的默认值为 `true` ）

`allowDisplayingInsecureContent` 表示是否允许一个使用 https 的界面来展示由 http URLs 传过来的资源。默认 `false`。

`allowRunningInsecureContent` 表示是否允许一个使用 https 的界面来渲染由 http URLs 提交的 html，css，javascript。默认为 `false`。