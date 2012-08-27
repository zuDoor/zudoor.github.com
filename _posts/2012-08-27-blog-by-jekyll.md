---
title: Blog by Jekyll
tags: blog markdown backbone
---

# Blog by Jekyll

一直用着github，却不知道其Page功能。昨天发现后，便捣鼓起来。[Jekyll][] 用来比较*KISS*，[Liquid][]也nice。起初，想用[Backbone][]做个Single-Page-App，用template把post转成json。代码写到当中，发现Backbone的View在对接上不是很简洁，尤其是使用[LayoutManager][]。

Jekyll的主旨就是把数据通过模板生产出可阅读的数据，及`Page = Template{data}`，这样整个功能逻辑就结束了。而Backbone的MCV是关注数据和显示的模块话，犹如`App = Route(View(Model(data)))`。前者在后端就已经混完了，后者要在后端把数据摘个干净。

两者的考虑方式是不同的，应用场景也有差异了。考虑到Page的Blog功能，在自动生产的代码上做了点修改，便成了现在的模样。如果有其他功能的添加，还是要试着Backbone来组合。

{% include ref.md %}
