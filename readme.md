## vue-blog-template

> 项目原本的初衷是描述我搭建自己学习blog的过程，以及我想通过blog去记录一些自己学习的经历。
> 但是前期记录这些文档，真是非常麻烦。最具体的例子就是**如果需要去摘记一些codes我得截图，或者是我得手写标签**
> 我觉得这毫无疑问是效率极低的。随着我学习webpack，我意识到有很多好的办法去解决这一问题。使用markdown文件去撰写日志，到最后我发现很多人都能使用。它不再局限于我个人的blog。

**所以，vue-blog-template诞生了**🎉🎉🎉

#### markdown

用markdown去写html页面这不是很cool的行为吗？这基于markdown-loader + html-loader，再配合highlight.js。
具体使用可以详见项目介绍

#### 侧边栏导航组件

通过更新cnav文件夹中的navList.js文件，修改侧边栏内容
例如
```
  {
    title: '标题',
    path: '',
    list: [
      { subtitle: '副标题', path: '对应url地址' }
    ]
  }
```

#### 适应小屏幕手机

具体你可以通过使用小屏幕手机来浏览下，当然这个响应式还是有弊端的。
因为通过了页面第一次加载时的生命周期判断用户的设备型号。所以你如果用chrome开发者模式选用手机浏览，它并未能响应布局。

#### plan

1. 完善README.md(也相当于完善项目介绍的那个markdown)
2. 整一下scss  @ues问题 这肯定和webpack脱不了关系
3. 写一个loader? highlight.js 和 markdown.js