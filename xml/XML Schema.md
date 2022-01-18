[XML Schema快速入门（一）如何使用_多学习多思考-CSDN博客](https://blog.csdn.net/weixin_41947378/article/details/104105408)
[XML Schema快速入门（二）语法之简单类型_多学习多思考-CSDN博客](https://blog.csdn.net/weixin_41947378/article/details/104091967)
[XML Schema快速入门（三）语法之复杂类型_多学习多思考-CSDN博客](https://blog.csdn.net/weixin_41947378/article/details/104138815)

# 什么是 XML [Schema](https://so.csdn.net/so/search?q=Schema&spm=1001.2101.3001.7020)？
> Schema，即XML Schema，XSD (XML Schema Definition)是W3C于2001年5月发布的推荐标准，指出如何形式描述XML文档的元素。XSD是许多XML Schema 语言中的一支。XSD是首先分离于XML本身的schema语言，故获取W3C的推荐地位。

XML Schema 是基于 XML 的 DTD 替代者。
XML Schema 的作用是定义 XML 文档的合法构建模块，类似 DTD。
XML Schema 语言也称作 XML Schema 定义（XML Schema Definition，XSD）。
注意：XSD只是Schema众多规范中的一种，还有XDR、DCD、SOX、DDML。

XML Scheman功能:

- 定义可出现在文档中的元素
- 定义可出现在文档中的属性
- 定义哪个元素是子元素
- 定义子元素的次序
- 定义子元素的数目
- 定义元素是否为空，或者是否可包含文本
- 定义元素和属性的数据类型
- 定义元素和属性的默认值以及固定值

————————————————

# 如何使用

本章主要讲解的是如何定义schema文件，以及如何在xml文件中引入schema约束，定义schema文件，可以定义有命名空间的和没有命名空间，对应的引入方式也有所不同。

## 1.定义没有命名空间的xsd文件

下面这个例子是名为 “books.xsd” 的schema文件，没有指定命名空间。不指定命名空间，该schema所申明的所有元素会默认归于无命名空间（无命名空间，将在讲解elementFormDefault属性的时候会说，可以先看[传送门](https://blog.csdn.net/weixin_41947378/article/details/104105408#elementFormDefault)）
