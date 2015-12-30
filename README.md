# Backbone
Backbone框架是典型的MVC框架，结构清晰。它是通过模型（model）和集合（collection）从服务器后台获取资源，然后在视图（view）中绑定这些资源，进行模板渲染，同时进行DOM事件处理配置，来避免DOM事件滥用。

优点：

1. 将业务逻辑和模板进行分离
2. 扩展性和维护性很好
3. 能很好的实现模块间的松耦合和事件驱动

缺点：

1. Model模型结构比较单一，一对多数据模型难以实现，用对象做属性也不行
2. 在view视图页面中容易产生内存泄露（比如通过 URL 切换改变整个页面时，页面上尚存的 View如何处理？直接销毁的话，是否要销毁关联的 Model、Collection？）

参考资料:

1. http://segmentfault.com/a/1190000002386651
2. http://segmentfault.com/a/1190000000465965#articleHeader0
3. http://segmentfault.com/a/1190000002666658
