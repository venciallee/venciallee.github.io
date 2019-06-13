---
title: 2019-06-05 30 Web Components
permalink: /web/Web Components/
layout: posts
last_modified_at: 2019-06-05T09:45:06-05:00
tags:
  - Web Components
categories:
  - Web Components
---

### 基础语法
- 声明式渲染

```javascript
  // HTML
  <div id="app-2">
    // v-bind将title特性和vue实例的message属性保持一致
    <span v-bind:title="message">
    </span>
  </div>

  // JS
  var app = new Vue({
    el:'#app-2',
    data: {
      message:'页面加载于' + new Date().toLocaleString();
    }
  })
```
- 条件循环

```javascript
  // HTML
  <div id="app-3">
    <p v-if="seen">现在你看到我了</p>
  </div>

  // JS
  var app = new Vuew({
    el:'#app-3',
    data: {
      seen: true
    }
  })
```

### 2.15.4 参考文档
- [Vue.js](https://cn.vuejs.org/v2/guide/)