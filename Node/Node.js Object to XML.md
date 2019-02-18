# Node.js Object to XML

有时我们需要给前端返回XML格式的数据，不幸的是这个过程并不像转换JSON那样方便，所以我们需要使用**xml2js**。

**xml2js**是支持Object和XML双向转换的，本文介绍的是序列化XML的过程。

### 安装xml2js
```javascript
npm install xml2js
```

### 创建XML
以创建一个RSS格式的XML为例，需要创建两个js文件：
RSSModel.js文件中定义RSS数据结构
index.js是主文件

```javascript
//RSSModel.js

function RSS() {
    this.$ = {version:'2.0'};
    this.channel = [new Channel()];
}

function Channel() {
    this.title = '';
    this.link = '';
    this.description = '';
}

exports.RSS = RSS;
exports.Channel = Channel;
```
这只是一个例子，所以不必在意数据结构的合理性，值得说明的是这行代码：

```javascript
this.$ = {version:'2.0'};
```
变量名定位为美元符号“$”，目的是把 *version* 视为为XML节点的属性，而不是值。

```javascript
<rss version="2.0"></rss>
```


```javascript
//index.js

const xml2js = require('xml2js');
const builder = new xml2js.Builder({rootName:'rss'}); //根节点定义为rss，默认是root
let rss = new RSSModel.RSS();
rss.channel[0].link = 'http://www.google.com';
rss.channel[0].title = 'google';
rss.channel[0].description = '谷歌';
const xmlStr = builder.buildObject(rss);
console.log(xmlStr);
```

```javascript
//输出

<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<rss version="2.0">
  <channel>
    <title>google</title>
    <link>http://www.google.com</link>
    <description>谷歌</description>
  </channel>
</rss>
```

更详细的使用方法请参看：[https://www.npmjs.com/package/xml2js](https://www.npmjs.com/package/xml2js)

---
*2018-12-21*

*by blues*