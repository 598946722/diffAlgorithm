## 虚拟 DOM 与 diff 算法的介绍与实现

```
单页应用一般都使用了各种diff算法使得SPA页面能够达到低消耗，快响应的目的。

SPA的主要特点在于“虚拟DOM”，至于什么是虚拟DOM，下文会介绍到。
```

### 虚拟 DOM 与真实 DOM

```
真实DOM即我们平时所写的HTML，而虚拟DOM则是通过JS读取数据结构，再根据数据结构渲染出真实DOM。
```

### 创建一个暴力更新的虚拟 DOM

1. [浅拷贝单节点暴力更新](./examples/demo01.html)

```
该示例根据一定的数据格式实现JS渲染生成真实的 HTML DOM,
通过JS浅拷贝实现单层HTML渲染。
```

1. [浅拷贝单层多节点暴力更新](./examples/demo02.html)

```
该示例根据一定的数据格式实现JS渲染生成真实的 HTML DOM,
通过JS浅拷贝实现单层HTML渲染。
```

2. [深拷贝多层多节点暴力更新](./examples/demo03.html)

```
该示例根据一定的数据格式实现JS渲染生成真实的 HTML DOM,
通过JS逐层渲染实现深拷贝多层HTML渲染。
```

3. 暴力更新的问题

```
1. 全结构渲染
2. 不管当前DOM是否变化，全部重新渲染绘制
3. 性能损耗严重
```

4. diff 的目的

```
区别全部渲染，只有第一次才全部渲染，并做节点标记，根据变化的节点进行单独更新，以达到性能提升的目的。
```

### 局部渲染 DOM

### 基于 Vue 的 diff 算法介绍

### 基于 React 的 diff 算法介绍
