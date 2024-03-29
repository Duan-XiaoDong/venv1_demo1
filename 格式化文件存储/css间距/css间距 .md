# CSS间距

### 内补白（内补丁）
```
padding： 检索或设置对象四边的内部边距,如padding:10px; padding:5px 10px;
padding-top： 检索或设置对象顶边的内部边距
padding-right： 检索或设置对象右边的内部边距
padding-bottom：检索或设置对象下边的内部边距
padding-left： 检索或设置对象左边的内部边距
```

### 外补白（外补丁）
```
margin： 检索或设置对象四边的外延边距,如 margin:10px; margin:5px auto;
margin-top： 检索或设置对象顶边的外延边距
margin-right： 检索或设置对象右边的外延边距
margin-bottom： 检索或设置对象下边的外延边距
margin-left： 检索或设置对象左边的外延边距
```
**margin相关技巧**
```angularjs
1、设置元素水平居中： margin:x auto;
2、margin负值让元素位移及边框合并
```


# 盒子模型

元素在页面中显示成一个方块，
类似一个盒子，CSS盒子模型就是使用现实中盒子来做比喻，
帮助我们设置元素对应的样式。

> 把元素叫做盒子，设置对应的样式分别为：
> 盒子的边框(border)、盒子内的内容和边框之间的间距(padding)、盒子与盒子之间的间距(margin)。

```angularjs
盒子真实尺寸
盒子宽度 = width + padding左右 + border左右
盒子高度 = height + padding上下 + border上下
```

在布局中，如果我想增大内容和边框的距离，又不想改变盒子显示的尺寸

```angularjs
box-sizing：content-box | border-box
```

# 块元素,内联元素,内联块元素

> 元素就是标签，布局中常用的有三种标签，块元素、内联元素、内联块元素，
>了解这三种元素的特性，才能熟练的进行页面布局。

### 块元素
块元素，也可以称为行元素，布局中常用的标签如：div、p、ul、li、h1~h6、dl、dt、dd等等都是块元素，
它在布局中的行为：

- 支持全部的样式
- 如果没有设置宽度，默认的宽度为父级宽度100%
- 盒子占据一行、即使设置了宽度

### 内联元素

内联元素，也可以称为行内元素，布局中常用的标签如：a、span、em、b、strong、i等等都是内联元素，它们在布局中的行为：

- 支持部分样式（不支持宽、高、margin上下）
- 宽高由内容决定
- 盒子并在一行
- 代码换行，盒子之间会产生间距
- 子元素是内联元素，父元素可以用text-align属性设置子元素水平对齐方式，用line-height属性值设置垂直对齐方式

### 内联块元素

内联块元素，也叫行内块元素，是新增的元素类型，现有元素没有归于此类别的，img和input元素的行为类似这种元素，但是也归类于内联元素，它们在布局中表现的行为：

- 支持全部样式
- 如果没有设置宽高，宽高由内容决定
- 盒子并在一行
- 代码换行，盒子会产生间距
- 子元素是内联块元素，父元素可以用text-align属性设置子元素水平对齐方式，用line-height属性值设置子元素垂直对齐方式

# 块元素,内联元素,内联块元素之间的转换

display属性是用来设置元素的类型及隐藏的，常用的属性有：

1、none 元素隐藏且不占位置

2、block 元素以块元素显示

3、inline 元素以内联元素显示

4、inline-block 元素以内联块元素显示