# 深入浅出 Webpack

[![img](https://ws1.sinaimg.cn/large/006tKfTcly1g0kvb1bfh4j30u014oqp1.jpg)](http://union-click.jd.com/jdc?d=1AMcaz)

## 评价

> Webpack 凭借强大的功能与良好的使用体验，已经成为目前最流行，社区最活跃的打包工具，是现代 Web 开发必须掌握的技能之一。作者结合自身的实战经验，介绍了 Webpack 的使用与常见优化方法、并深入讲解了 Webpack 原理与架构，相信各阶段的 Webpack 用户都能通过本书得到启发。
>
> -- [LeanCloud](https://leancloud.cn/?source=00YQRYTC) 联合创始人/CEO 江宏
>
> 本书的内容包含多个主题，Webpack 的用法、配置、使用场景等都有涉及，并且提供所有示例的源码，可以补充 Webpack 官方文档。
>
> -- 阮一峰（[著名技术博客](http://www.ruanyifeng.com/blog/)，[《ES6 标准入门》](http://union-click.jd.com/jdc?d=Vaj3NC)的作者）
>
> 我手边需要这样一本书，内容涵盖Webpack，或者说涵盖现代前端技术基础、构建与优化的方方面面。如果你已经上手 Webpack，那么本书将带领你进一步学习，真正掌握 Webpack！
>
> -- 陆金所前端架构师、[前端外刊评论](https://qianduan.group/)站长 寸志

## 版权许可

电子工业出版社持有本书全媒体形式的出版发行权利。

[吴浩麟](https://github.com/gwuhaolin)拥有本书的著作权。

**其它人不能将本书用于商用用途，不能转载，不能以任何形式发行，违者将追究法律责任**。

## 目录

- [前言](http://webpack.wuhaolin.cn/%E5%89%8D%E8%A8%80.html)

### [第1章 入门](http://webpack.wuhaolin.cn/1%E5%85%A5%E9%97%A8/)

- [1-1 前端的发展](http://webpack.wuhaolin.cn/1%E5%85%A5%E9%97%A8/1-1%E5%89%8D%E7%AB%AF%E7%9A%84%E5%8F%91%E5%B1%95.html)
- [1-2 常见的构建工具及对比](http://webpack.wuhaolin.cn/1%E5%85%A5%E9%97%A8/1-2%E5%B8%B8%E8%A7%81%E7%9A%84%E6%9E%84%E5%BB%BA%E5%B7%A5%E5%85%B7%E5%8F%8A%E5%AF%B9%E6%AF%94.html)
- [1-3 安装与使用](http://webpack.wuhaolin.cn/1%E5%85%A5%E9%97%A8/1-3%E5%AE%89%E8%A3%85%E4%B8%8E%E4%BD%BF%E7%94%A8.html)
- [1-4 使用 Loader](http://webpack.wuhaolin.cn/1%E5%85%A5%E9%97%A8/1-4%E4%BD%BF%E7%94%A8Loader.html)
- [1-5 使用 Plugin](http://webpack.wuhaolin.cn/1%E5%85%A5%E9%97%A8/1-5%E4%BD%BF%E7%94%A8Plugin.html)
- [1-6 使用 DevServer](http://webpack.wuhaolin.cn/1%E5%85%A5%E9%97%A8/1-6%E4%BD%BF%E7%94%A8DevServer.html)
- [1-7 核心概念](http://webpack.wuhaolin.cn/1%E5%85%A5%E9%97%A8/1-7%E6%A0%B8%E5%BF%83%E6%A6%82%E5%BF%B5.html)

### [第2章 配置](http://webpack.wuhaolin.cn/2%E9%85%8D%E7%BD%AE/)

- [2-1 Entry](http://webpack.wuhaolin.cn/2%E9%85%8D%E7%BD%AE/2-1Entry.html)
- [2-2 Output](http://webpack.wuhaolin.cn/2%E9%85%8D%E7%BD%AE/2-2Output.html)
- [2-3 Module](http://webpack.wuhaolin.cn/2%E9%85%8D%E7%BD%AE/2-3Module.html)
- [2-4 Resolve](http://webpack.wuhaolin.cn/2%E9%85%8D%E7%BD%AE/2-4Resolve.html)
- [2-5 Plugins](http://webpack.wuhaolin.cn/2%E9%85%8D%E7%BD%AE/2-5Plugins.html)
- [2-6 DevServer](http://webpack.wuhaolin.cn/2%E9%85%8D%E7%BD%AE/2-6DevServer.html)
- [2-7 其它配置项](http://webpack.wuhaolin.cn/2%E9%85%8D%E7%BD%AE/2-7%E5%85%B6%E5%AE%83%E9%85%8D%E7%BD%AE%E9%A1%B9.html)
- [2-8 整体配置结构](http://webpack.wuhaolin.cn/2%E9%85%8D%E7%BD%AE/2-8%E6%95%B4%E4%BD%93%E9%85%8D%E7%BD%AE%E7%BB%93%E6%9E%84.html)
- [2-9 多种配置类型](http://webpack.wuhaolin.cn/2%E9%85%8D%E7%BD%AE/2-9%E5%A4%9A%E7%A7%8D%E9%85%8D%E7%BD%AE%E7%B1%BB%E5%9E%8B.html)
- [2-10 配置总结](http://webpack.wuhaolin.cn/2%E9%85%8D%E7%BD%AE/2-10%E9%85%8D%E7%BD%AE%E6%80%BB%E7%BB%93.html)

### [第3章 实战](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/)

- [3-1 使用 ES6 语言](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-1%E4%BD%BF%E7%94%A8ES6%E8%AF%AD%E8%A8%80.html)
- [3-2 使用 TypeScript 语言](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-2%E4%BD%BF%E7%94%A8TypeScript%E8%AF%AD%E8%A8%80.html)
- [3-3 使用 Flow 检查器](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-3%E4%BD%BF%E7%94%A8Flow%E6%A3%80%E6%9F%A5%E5%99%A8.html)
- [3-4 使用 SCSS](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-4%E4%BD%BF%E7%94%A8SCSS%E8%AF%AD%E8%A8%80.html)
- [3-5 使用 PostCSS](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-5%E4%BD%BF%E7%94%A8PostCSS.html)
- [3-6 使用 React 框架](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-6%E4%BD%BF%E7%94%A8React%E6%A1%86%E6%9E%B6.html)
- [3-7 使用 Vue 框架](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-7%E4%BD%BF%E7%94%A8Vue%E6%A1%86%E6%9E%B6.html)
- [3-8 使用 Angular2 框架](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-8%E4%BD%BF%E7%94%A8Angular2%E6%A1%86%E6%9E%B6.html)
- [3-9 为单页应用生成 HTML](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-9%E4%B8%BA%E5%8D%95%E9%A1%B5%E5%BA%94%E7%94%A8%E7%94%9F%E6%88%90HTML.html)
- [3-10 管理多个单页应用](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-10%E7%AE%A1%E7%90%86%E5%A4%9A%E4%B8%AA%E5%8D%95%E9%A1%B5%E5%BA%94%E7%94%A8.html)
- [3-11 构建同构应用](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-11%E6%9E%84%E5%BB%BA%E5%90%8C%E6%9E%84%E5%BA%94%E7%94%A8.html)
- [3-12 构建 Electron 应用](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-12%E6%9E%84%E5%BB%BAElectron%E5%BA%94%E7%94%A8.html)
- [3-13 构建 Npm 模块](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-13%E6%9E%84%E5%BB%BANpm%E6%A8%A1%E5%9D%97.html)
- [3-14 构建离线应用](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-14%E6%9E%84%E5%BB%BA%E7%A6%BB%E7%BA%BF%E5%BA%94%E7%94%A8.html)
- [3-15 搭配 Npm Script](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-15%E6%90%AD%E9%85%8DNpmScript.html)
- [3-16 检查代码](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-16%E6%A3%80%E6%9F%A5%E4%BB%A3%E7%A0%81.html)
- [3-17 通过 Node.js API 启动 Webpack](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-17%E9%80%9A%E8%BF%87Node.jsAPI%E5%90%AF%E5%8A%A8Webpack.html)
- [3-18 使用 Webpack Dev Middleware](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-18%E4%BD%BF%E7%94%A8WebpackDevMiddleware.html)
- [3-19 加载图片](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-19%E5%8A%A0%E8%BD%BD%E5%9B%BE%E7%89%87.html)
- [3-20 加载SVG](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-20%E5%8A%A0%E8%BD%BDSVG.html)
- [3-21 加载 Source Map](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-21%E5%8A%A0%E8%BD%BDSourceMap.html)
- [3-22 实战总结](http://webpack.wuhaolin.cn/3%E5%AE%9E%E6%88%98/3-22%E5%AE%9E%E6%88%98%E6%80%BB%E7%BB%93.html)

### [第4章 优化](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/)

- [4-1 缩小文件搜索范围](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/4-1%E7%BC%A9%E5%B0%8F%E6%96%87%E4%BB%B6%E6%90%9C%E7%B4%A2%E8%8C%83%E5%9B%B4.html)
- [4-2 使用 DllPlugin](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/4-2%E4%BD%BF%E7%94%A8DllPlugin.html)
- [4-3 使用 HappyPack](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/4-3%E4%BD%BF%E7%94%A8HappyPack.html)
- [4-4 使用 ParallelUglifyPlugin](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/4-4%E4%BD%BF%E7%94%A8ParallelUglifyPlugin.html)
- [4-5 自动刷新与模块热替换](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/4-5%E4%BD%BF%E7%94%A8%E8%87%AA%E5%8A%A8%E5%88%B7%E6%96%B0.html)
- [4-6 开启模块热替换](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/4-6%E5%BC%80%E5%90%AF%E6%A8%A1%E5%9D%97%E7%83%AD%E6%9B%BF%E6%8D%A2.html)
- [4-7 区分环境](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/4-7%E5%8C%BA%E5%88%86%E7%8E%AF%E5%A2%83.html)
- [4-8 压缩代码](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/4-8%E5%8E%8B%E7%BC%A9%E4%BB%A3%E7%A0%81.html)
- [4-9 CDN 加速](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/4-9CDN%E5%8A%A0%E9%80%9F.html)
- [4-10 使用 Tree Shaking](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/4-10%E4%BD%BF%E7%94%A8TreeShaking.html)
- [4-11 提取公共代码](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/4-11%E6%8F%90%E5%8F%96%E5%85%AC%E5%85%B1%E4%BB%A3%E7%A0%81.html)
- [4-12 按需加载](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/4-12%E6%8C%89%E9%9C%80%E5%8A%A0%E8%BD%BD.html)
- [4-13 使用 Prepack](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/4-13%E4%BD%BF%E7%94%A8Prepack.html)
- [4-14 开启 Scope Hoisting](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/4-14%E5%BC%80%E5%90%AFScopeHoisting.html)
- [4-15 输出分析](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/4-15%E8%BE%93%E5%87%BA%E5%88%86%E6%9E%90.html)
- [4-16 优化总结](http://webpack.wuhaolin.cn/4%E4%BC%98%E5%8C%96/4-16%E4%BC%98%E5%8C%96%E6%80%BB%E7%BB%93.html)

### [第5章 原理](http://webpack.wuhaolin.cn/5%E5%8E%9F%E7%90%86/)

- [5-1 工作原理概括](http://webpack.wuhaolin.cn/5%E5%8E%9F%E7%90%86/5-1%E5%B7%A5%E4%BD%9C%E5%8E%9F%E7%90%86%E6%A6%82%E6%8B%AC.html)
- [5-2 输出文件分析](http://webpack.wuhaolin.cn/5%E5%8E%9F%E7%90%86/5-2%E8%BE%93%E5%87%BA%E6%96%87%E4%BB%B6%E5%88%86%E6%9E%90.html)
- [5-3 编写 Loader](http://webpack.wuhaolin.cn/5%E5%8E%9F%E7%90%86/5-3%E7%BC%96%E5%86%99Loader.html)
- [5-4 编写 Plugin](http://webpack.wuhaolin.cn/5%E5%8E%9F%E7%90%86/5-4%E7%BC%96%E5%86%99Plugin.html)
- [5-5 调试 Webpack](http://webpack.wuhaolin.cn/5%E5%8E%9F%E7%90%86/5-5%E8%B0%83%E8%AF%95Webpack.html)
- [5-6 原理总结](http://webpack.wuhaolin.cn/5%E5%8E%9F%E7%90%86/5-6%E5%8E%9F%E7%90%86%E6%80%BB%E7%BB%93.html)

### 附录

- [常用 Loaders](http://webpack.wuhaolin.cn/%E9%99%84%E5%BD%95/%E5%B8%B8%E7%94%A8Loaders.html)
- [常用 Plugins](http://webpack.wuhaolin.cn/%E9%99%84%E5%BD%95/%E5%B8%B8%E7%94%A8Plugins.html)
- [其它 Webpack 学习资源](http://webpack.wuhaolin.cn/%E9%99%84%E5%BD%95/%E5%85%B6%E5%AE%83Webpack%E5%AD%A6%E4%B9%A0%E8%B5%84%E6%BA%90.html)

------

[![img](https://ws2.sinaimg.cn/large/006tKfTcly1g0kvb1yty5j30qy05d74j.jpg)](https://leancloud.cn/?source=00YQRYTC)