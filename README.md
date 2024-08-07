# 仿钉钉后台审批流程
<p align="center" style="margin-bottom: 0 !important">
	<img alt="logo" src="https://gitee.com/ldhnet/AntFlow-Vue3/raw/master/public/images/logo.png"  width = "80px"; height= "80px";>
</p>
<h1 align="center" style="margin: 10px 10px; font-weight: bold;margin-top: 0 !important">AntFlow-Vue2</h1>
<h4 style="border-top: solid #ACC0D8 1px;"></h4>
<h4 align="center">AntFlow-Vue2是基于Vue2 的前端工作流配置新模式 </h4>
<h4 align="center" style="margin: 0px 0px 30px 10px; ">
后端自主研发基于SpringBoot + Activiti 开发的轻量级工作流框架</h4>

- 特此声明 完全开源，开源不易，点个星星支持一下。

- Ant-Flow Vue3 版本[预览入口](http://117.72.70.166/ant-flow/dist/#/)

- Ant-Flow Vue3 版本[Gitee仓库](https://gitee.com/ldhnet/AntFlow-Vue3)

- QQ技术交流群（972107977）期待您的加入
 

基于JakHuang大佬的[form-generator](https://github.com/JakHuang/form-generator)的，仿钉钉后台审批流程创建界面

## 安装使用
 
- 安装依赖
yarn install | npm install

- 运行
yarn serve | npm run serve

- 打包
yarn build  | npm run build

- 本地预览
yarn preview 

- 打包/预览 
yarn build:preview 

## 主要功能
1. 表单配置(form-generator)
  - 拖拽表单，生成布局页面
  - 配置拖拽组件属性，定制组件形态
  - 生成JSON数据并生成预览页面
2. 流程节点配置(仿钉钉界面)
  - 创建审批流程(发起人，审批人，条件节点，抄送人)
  - 配置节点详细数据，包括条件节点表达式及期望值等
  - 配置节点对表单得权限（目前并未在预览页面中做控制）
  - 必填节点校验

## 基本结构
```
// src
|-- components
|---- BasicSetting // 基础设置
|---- DynamicForm      // 表单配置
|---- Process          // 流程配置
|---- AdvancedSetting  // 高级设置
|---- FormControls     // 扩充表单组件

|-- views
|---- admin  // 后台配置界面
|---- custom // 前台预览界面
```
> 不想把JakHuang大佬的项目拆分出来 一是为了方便学习大佬代码 二是为了以后单独抽离表单出来更方便 所以没有把form-generator项目的公用文件抽离到顶层 流程创建组件同理

## 表单组件
1. 单行输入框, 多行输入框, 数字输入框, 金额
2. 下拉选择, 级联选择, 省市区
3. 单选框组, 多选框组
4. 时间选择, 时间范围, 日期选择, 日期范围
5. 滑块, 组织机构, 附件, 计算公式
6. 布局容器, 表格/列表

## 界面预览
![YL5ip8.png](https://s1.ax1x.com/2020/05/22/YL5ip8.png)
![YL5k6g.png](https://s1.ax1x.com/2020/05/22/YL5k6g.png)
![YL5Cff.png](https://s1.ax1x.com/2020/05/22/YL5Cff.png)
![YL5F1S.png](https://s1.ax1x.com/2020/05/22/YL5F1S.png)
![YL5Z0s.png](https://s1.ax1x.com/2020/05/22/YL5Z0s.png)
![YL5Vmj.png](https://s1.ax1x.com/2020/05/22/YL5Vmj.png)
 




