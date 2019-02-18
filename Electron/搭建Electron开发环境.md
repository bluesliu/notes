# 搭建 Electron 开发环境

## 创建项目

```shell
# github上有一个 electron-quick-start 仓库克隆下来
git clone https://github.com/electron/electron-quick-start
# 进入文件夹
cd electron-quick-start
# 安装依赖包并运行
npm install && npm start
```



## WebStorm 调试

1. 进入菜单：`Run/Edit Configurations...`
2. 新建`Node.js`调试配置
3. `Node interpreter` 下拉列表选 `Add...` →`Add Local…`；在弹出的`Select Path`窗口中选择路径：`当前项目路径/node_modules/.bin/electron`
4. `Node parameters`填写`.`
5. 点击`OK`按钮完成

![屏幕快照 2019-02-18 上午11.26.05](/Users/blues/Documents/md/notes/Electron/assets/屏幕快照 2019-02-18 上午11.26.05.png)