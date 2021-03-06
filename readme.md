简体中文 | [English](./README.zh-English.md) 

<div align="center">

![](https://github.com/welkin-qing/todomvc-vue/blob/master/img/mylogo.png)

一个基于 Vue 框架开发的 ToDoMVC 实例

An instance of ToDoMVC based on Vue

![](https://github.com/welkin-qing/todomvc-vue/blob/master/img/release-1.0-darkcyan.svg)
![](https://github.com/welkin-qing/todomvc-vue/blob/master/img/build-passing-brightgreen.svg)
![](https://github.com/welkin-qing/todomvc-vue/blob/master/img/dependencies-up%20to%20date-brightgreen.svg)
![](https://github.com/welkin-qing/todomvc-vue/blob/master/img/license-MIT-darkcyan.svg)

</div>

-----

# 安装及使用
```js
git clone git@github.com:welkin-qing/todomvc-vue.git
cd todomvc-vue
npm install
npm run dev/ npm start
```
-----

# 基本配置
### 下载ToDoMVC模板
https://github.com/tastejs/todomvc-app-template
### 配置browser-sync浏览器同步测试工具及配置scripts

```js
cnpm install --save-dev browser-sync
```
# 基本作用
###  添加任务
1. 敲回车添加到任务列表中
2. 判断是否为非空数据，若是，则不添加；添加完成后清空文本框

### 任务项
1. 联动样式，切换任务完成状态
2. 删除任务项
3. 双击label编辑任务项

### 编辑任务项
1. 编辑文本自动获得焦点(使用自定义指令)
2. 敲回车或者失去焦点则保存文本
3. 输入状态下，esc取消编辑
4. 显示所有未完成数；点击清除完成项，清除所有已完成任务（使用计算属性）

### 数据持久化
1. 将数据持久化到localStorage，实现本地存储
2. 使用watch监视数据的改变，删除，增加

### 路由切换状态
1. 点击链接过滤数组的输出（使用hash）
2. 刷新保持过滤状态
3. 切换点击链接的样式

### 自定义指令获得焦点
1. 使用全局指令使页面一上来就获得焦点（以后不需要）
2. 使用指令获得作用到该指令的Dom元素，使其获得焦点

###### 注意
cnpm install --production 可以只装dependencies中的包
