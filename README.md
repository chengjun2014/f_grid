# Grid 
----
> 基于`bootstrap`第三版
> @只能使用 md 或 lg；类格式：col-@-x

## 文档说明

最终生成的grid分别为24列(lg)和20列(md)，列间距固定20px;

类名：col-lg-x ("x"表示1-24)

      col-md-x ("x"表示1-20)

## 结构

仍然按照`bootstrap`官方对结构的要求("@"表示md或lg)

row: 表示行,概念类似于 div

row 作为`col-@-x`元素的父级元素，row 可以嵌套使用

col: 表示行内所占的列数，比如`col-md-3`: 表示站当前 row 的 3/20

*注*：`md`沿用自`bootstrap`官方，另可用`lg`参考`./index.less`源码

## 自定义
*row需要放在一个定宽容器内* 

后续可能需要修改变量值文件目录是`./variables.less`

目前尺寸沿用的是`bootstrap`官方尺寸，比如 container 宽度为 1200px

## 源码来自`bootstrap`官方精简版

如果需要其他`bootstrap`扩展功能需要另外引入对应的样式预编译代码，

目前只引用了 grid 部分代码，保证最小可用

## 可用类名
.row：表示一行

.col-@-x：当前元素所占最近row的 x/(20|24) * 100% 宽度

.col-@-pull-x: (还有.col-@-pull-0) 影响当前元素的 right 属性

.col-@-push-x: (还有.col-@-push-0) 影响当前元素的 left 属性

.col-@-offset-x: (还有.col-@-offset-0) 影响当前元素的 margin-left 属性

## 框架标准化
框架标准化的推动需要设计师的配合；

设计上要求各模块、元素尺寸符合1/(20|24)的整数倍

## 参考资源
`bootstrap`官方网站: http://www.bootcss.com/

`Less`官网：http://www.lesscss.cn/

