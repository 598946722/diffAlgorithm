## 虚拟 DOM 与 diff 算法的介绍与实现

```
单页应用一般都使用了各种diff算法使得SPA页面能够达到低消耗，快响应的目的。

SPA的主要特点在于“虚拟DOM”，至于什么是虚拟DOM，下文会介绍到。
```

### 创建一个暴力更新的虚拟 DOM

1. [浅拷贝暴力更新](./examples/demo01.html)

```seq
div -> div
```

```
该示例根据一定的数据格式实现JS渲染生成真实的 HTML DOM,
通过JS浅拷贝实现单层HTML渲染。
```

2. [深拷贝暴力更新](./examples/demo01.html)

```
该示例根据一定的数据格式实现JS渲染生成真实的 HTML DOM,
通过JS逐层渲染实现深拷贝多层HTML渲染。
```

3. 暴力更新的性能分析

```

```

### 基于 Vue 的 diff 算法介绍

### 基于 React 的 diff 算法介绍
