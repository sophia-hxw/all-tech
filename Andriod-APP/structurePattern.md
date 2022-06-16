## MVC架构
Model View Controller，即模型-视图-控制器，使用MVC的目的是将M和V的实现代码分离，从而使同一个程序可以使用不同的表现形式。

## MVP架构
Model View Presenter，即模型-视图-表示器，在MVP中，View不直接与Model交互，它们之间通信用Presenter实现。

## MVVM架构
Model View ViewModel，ViewModel就相当于MVP中的Presenter和MVC中的Controller，而View与ViewModel直接交互，用数据“绑定”的形式实现数据双向同步。

## MVP+VM架构
MVVM与MVP相比，优化了数据频繁更新的解决方案，但某种程度上又把View和Model耦合在一起了。在实际应用中，往往是把MVP脚骨和DataBinding技术一起使用。




