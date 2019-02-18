# Node.js 命令行开发

读了阮一峰老师的[《Node.js 命令行程序开发教程》](http://www.ruanyifeng.com/blog/2015/05/command-line-with-node.html)教程，受益颇丰。熟练运用这一技能可以开发很多自动化工具，大大提高效率。



## 创建可自行脚本

1. 创建名为 hello 的脚本

```javascript
#!/usr/bin/env node
console.log('hello world');
```

2. 创建 package.json

```json
{
  "name": "hello",
  "bin": {
    "hello": "hello"
  }
}
```

3. 使用 npm link 命令

```shell
$ npm link
```

以上步骤完成后，就可以直接在命令行输入：`hello`看效果了。

![屏幕快照 2019-02-18 下午4.45.45](https://ws2.sinaimg.cn/large/006tKfTcgy1g0ao7pvfnvj311w0qidpc.jpg)

创建了自己的命令行工具真的很酷。其实`hello`脚本就作为一个全局模块安装到了`usr⁩/local/lib/node_modules`目录下。

   

## 卸载

```shell
$ npm unlink hello -g
```

