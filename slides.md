---
theme: default
class: "text-center"
highlighter: shiki
lineNumbers: false
info: |
  ## Atomic components design
drawings:
  persist: false
---

# Components Development

---

# Problems

- 项目结构混乱
- elementUI 修改样式困难
- 分工困难

```
.el-input-number .el-input__inner {
  text-align: left !important;
}

```

---

# Atomic design

<img src="/assets/atomic_design.png" class="w-full">

[Link](https://atomicdesign.bradfrost.com/chapter-2/)
<br>
<br>

<!--
atoms 原子组件
molecules 分子组件
organisms 有机体组件
templates 布局组件
pages 页面
-->

---

# Architecture

<div grid="~ cols-3 gap-4 pt-30"> 
  <div> 
    <h2> Pages </h2> 
    <ul>
      <li> 基于路由 </li>
      <li> Layout(Template) </li>
      <li> 获取数据(AsyncData) </li>
    </ul>
  </div>
  <div>
    <h2> Blocks </h2>
    <ul>
      <li> Organisms </li>
      <li> 获取数据(Fetch) </li>
    </ul>
  </div>
  <div>
    <h2> Components </h2>
    <ul>
      <li> Atoms & Molecules </li>
      <li> Reusable </li>
      <li> 与数据无关 </li>
    </ul>
  </div>
</div>

---

# Component

- 原子组件(参考基础组件修改样式)
- 基于 Storybook 开发
- 与后端数据无关

---

# Design style

基于 scss 全局变量实现

- **Color**
- **Fonts**
- **Layout**

---

# Recommand 


- [Logbook](https://github.com/thematters/logbook)

- [Atomic Design](https://atomicdesign.bradfrost.com/)

- [Inkline](https://github.com/inkline/inkline)
