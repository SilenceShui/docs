# Markdown 基础语法

> #### 标题

```markdown
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

# 一级标题

## 二级标题

### 三级标题

#### 四级标题

##### 五级标题

###### 六级标题

> #### 字体

```markdown
*斜体文本*
_斜体文本_
**粗体文本**
__粗体文本__
***粗斜体文本***
___粗斜体文本___
```

*斜体文本*   

_斜体文本_  

**粗体文本**  

__粗体文本__  

***粗斜体文本***  

___粗斜体文本___  

> #### 分割线

```markdown
***

* * *

*****

- - -

----------
```

***

* * *

*****

- - -

----------

> #### 删除线、下划线

```markdown
~~BAIDU.COM~~
<u>带下划线文本</u>
```

~~BAIDU.COM~~

<u>带下划线文本</u>

> #### 列表

```markdown
无序列表
 * 第一项

 + 第二项

 - 第三项

有序列表
 1. 第一项
 2. 第二项
 3. 第三项

组合列表
 1. 第一项：
     - 第一项嵌套的第一个元素
     - 第一项嵌套的第二个元素
  2. 第二项：
     - 第二项嵌套的第一个元素
     - 第二项嵌套的第二个元素
```

###### 无序列表

- 第一项

- 第二项

- 第三项

###### 有序列表

1. 第一项
2. 第二项
3. 第三项

###### 组合列表

1. 第一项：
   - 第一项嵌套的第一个元素
   - 第一项嵌套的第二个元素
     2. 第二项：
   - 第二项嵌套的第一个元素
   - 第二项嵌套的第二个元素

> #### 区块

```markdown
> 区块引用1
> 区块引用2

> 最外层
> > 第一层嵌套
> > > 第二层嵌套

> 区块中使用列表
> 1. 第一项
> 2. 第二项
> + 第一项
> + 第二项
> + 第三项
```

> 区块引用1
> 区块引用2

> 最外层
> 
> > 第一层嵌套
> > 
> > > 第二层嵌套

> 区块中使用列表
> 
> 1. 第一项
> 2. 第二项
> - 第一项
> - 第二项

> #### 代码

```markdown
1 使用``包裹
2 代码区块使用 4 个空格
3 ``` 代码类型
    包裹代码
```

```javascript
$(document).ready(function () {
   console.log("hello world")
});
```

```
> #### 链接

```markdown
[链接名称](链接地址)
或者
<链接地址>
```

[百度一下](https://www.baidu.com)

<https://www.baidu.com>

> #### 图片

```markdown
![alt 属性文本](图片地址 "可选标题")
```

![山水画](./images/1.jpg)

> #### Markdown 表格

```markdown
-: 设置内容和标题栏居右对齐。
:- 设置内容和标题栏居左对齐。
:-: 设置内容和标题栏居中对齐。

| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |
```

| 左对齐 | 右对齐 | 居中对齐 |
|:--- | ---:|:----:|
| 单元格 | 单元格 | 单元格  |
| 单元格 | 单元格 | 单元格  |

> #### 转义

```markdown
**文本加粗** 
\*\* 正常显示星号 \*\*
```
