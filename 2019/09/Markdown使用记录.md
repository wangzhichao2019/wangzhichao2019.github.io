# Markdown使用记录

### 1.简介：

- __<font>大体介绍：</font>__
    - Markdown 是一种轻量级标记语言，它允许人们使用易读易写的纯文本格式编写文档。 
    - Markdown 语言在 2004 由约翰·格鲁伯（英语：John Gruber）创建。
    - Markdown 编写的文档可以导出 HTML 、Word、图像、PDF、Epub 等多种格式的文档。
    - Markdown 编写的文档后缀为 .md, .markdown。
- __<font>Markdown应用：</font>__
    - Markdown 能被使用来撰写电子书，如：Gitbook。
    - 当前许多网站都广泛使用 Markdown 来撰写帮助文档或是用于论坛上发表消息。例如：GitHub、简书、CSDN，还有我写这篇文章所用的工具Jupyter notebook
- __<font>编辑器：</font>__
    - 使用Typora编辑器来练习Markdown的语法，Typora支持MacOs、Linux、Windows平台，且包含多种主题，编辑后直接渲染出效果
    - 支持导出HTML、PDF、Word、图片等多种类型文件
    - Typora官网：https://typora.io/

### 2.Markdown标题：

#### 使用=和-标记一级和二级标题

- =和-标记语法格式如下：
我展示的是一级标题
=================

我展示的是二级标题
-----------------
- 显示效果如下：
![image.png](attachment:image.png)

### 3.Markdown段落

Markdown段落没有特殊的格式，直接编写文字就好，段落的换行是使用__<font color = red>两个及以上的空格加回车。</font>__
![image.png](attachment:image.png)

**字体**：Markdown可以使用以下几种字体
*斜体文本*
_斜体文本_
**粗体文本**
__粗体文本__
***粗斜体文本***
___粗斜体文本___
**分隔线**：你可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。你也可以在星号或是减号中间插入空格。
下面的每种写法都是可以的：
***

* * *

*****

- - - 

--------
显示效果如下：
![image.png](attachment:image.png)

__删除线__：如果段落上的文字要添加删除线，只需要在文字的两端家伙是哪个两个波浪线~~即可：
RUNOOB.COM
GOOGLE.COM
~~BAIDU.COM~~
**下划线**：可以通过HTML的<u>标签来实现：  
<u>带下划线的文本</u>
显示效果如下所示：
![image.png](attachment:image.png)

**脚注**：是对文本的补充说明。

Markdown脚注的格式如下：
[^要注明的文本]

创建脚注格式类似这样 [^RUNOOB]。  
[^RUNOOB]: 菜鸟教程 -- 学的不仅是技术，更是梦想！！！

演示效果：
![image.png](attachment:image.png)

### 4.Markdown区块

Markdown区块引用是在段落开头使用>符号，然后后面紧跟一个空格符号：
>区块引用   
>Jupyter实验中   
>学的不仅是技术更是梦想   
显示结果如下：

>区块引用   
>Jupyter实验中   
>学的不仅是技术更是梦想  

另外区块是可以嵌套的，一个>符号是最外层，两个>符号是第一层嵌套，以此类推
>最外层
>>第一层嵌套
>>>第二层嵌套
显示结果如下：

>最外层
>>第一层嵌套
>>>第二层嵌套

**区块中使用列表**   
区块中使用列表实例如下：
>区块中使用列表   
>1.第一项   
>2.第二项   
>- 第一项  
>+ 第二项  
>* 第三项  
显示结果如下：
>区块中使用列表   
>1.第一项   
>2.第二项   
>- 第一项  
>+ 第二项  
>* 第三项  

__列表中自然也可以使用区块:__

如果要在列表项目中放进区块，那么就需要在>前添加四个空格的缩进   
区块中使用列表实例如下：
* 第一项
    > Study
    > https://wangzhichao2019.github.io
    > 利用hexo在github上搭建的个人博客
* 第二项
* 第一项
    > Study
    > https://wangzhichao2019.github.io
    > 利用hexo在github上搭建的个人博客
* 第二项

### 5.Markdown代码：

如果是段落上的一个函数或片段的代码可以用反引号把它包起来（`）
例如： `printf()孤独的国`

显示结果如下：

`printf()孤独的国`

**代码区段**：使用四个空格或者是一个制表符（Tab键）  
实例如下：

    <?php
        echo '孤独的国'
        function test()
        {
            echo 'test'
        }
    ?>

也可以使用```包裹一段diamante，并指定一种语言（也可以不指定）:

```C++
    #include <iostream>
    using namespace std;
    int main()
    {
       int a,b;
       a = 10;
       b = 5;
       for(; b <= a; b++)
       {
          cout<<"访问https://wangzhichao2019.github.io"<<endl;
       }
       cout<<"大概一年的时间没有写C++代码了"<<endl;
    }

### 6.Markdown链接
链接使用方法如下：
    [链接名称](链接地址)
    
    或者
    
    <链接地址>例如：
这是一个链接[孤独的国](https://wangzhichao2019.github.io)
直接使用链接地址：
<https://wangzhichao2019.github.io>
显示结果如下：   
这是一个链接[孤独的国](https://wangzhichao2019.github.io)

<https://wangzhichao2019.github.io>
**高级链接**：
- 链接也可以用变量来代替，文档末尾附带变量地址：  
- 这个链接用1作为网址变量[Google](1)   
- 这个链接用"孤独的国"作为网址变量[hexo](孤独的国) 
- 然后在文档的结尾为变量赋值（网址）  

    (1):https://www.google.com
    
    (孤独的国):https://wangzhichao2019.github.io
**高级链接**：
- 链接也可以用变量来代替，文档末尾附带变量地址：  
- 这个链接用1作为网址变量[Google](1)   
- 这个链接用"孤独的国"作为网址变量[hexo](孤独的国) 
- 然后在文档的结尾为变量赋值（网址）  

    (1):https://www.google.com/
    
    (孤独的国):https://wangzhichao2019.github.io/

### 7.Markdown图片
Markdown图片语法格式如下：
![alt 属性文本](图片地址)
![alt 属性文本](图片地址 "可选标题")
- 开头一个感叹号 !
- 接着一个方括号，里面放上图片的替代文字
- 接着一个普通括号，里面放上图片的网址，最后还可以用引号包住并加上选择性的 'title' 属性的文字。
使用实例：   
![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png)

![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png "RUNOOB")
显示结果如下：

![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png)

![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png "RUNOOB")
当然，也可以像网址那样对图片网址使用变量:

这个链接用 1 作为网址变量 [RUNOOB][1].
然后在文档的结尾位变量赋值（网址）

[1]: http://static.runoob.com/images/runoob-logo.png
显示结果如下：

这个链接用 1 作为网址变量 [RUNOOB][1].
然后在文档的结尾位变量赋值（网址）

[1]: http://static.runoob.com/images/runoob-logo.png
Markdown还没有办法指定图片的高度和宽度，如果需要的话，可以使用普通的<img>标签

<img src="http://static.runoob.com/images/runoob-logo.png" width="50%">
显示结果如下：
<img src="http://static.runoob.com/images/runoob-logo.png" width="50%">

### 8.Markdown表格

Markdown制作表格使用|来分隔不同的单元格，使用-来分隔表头和其他行。
语法格式如下： 
| 表头| 表头|
|----|  ---- |
|单元格|单元格|
|单元格|单元格|
以上代码显示结果如下：   
语法格式如下： 

|  表头   || 表头  |
|  ----   || ----  |
| 单元格  || 单元格 |
| 单元格  || 单元格 |

**对齐方式**：   
__我们可以设置表格的对齐方式__:   
- -: 设置内容和标题栏居右对齐。

- :- 设置内容和标题栏居左对齐。

- :-: 设置内容和标题栏居中对齐。
实例如下：
| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |
| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |

### 9.Markdown高级技巧：
**支持的HTML元素**   
不在Markdown涵盖范围之内的标签，都可以直接在文档里面用HTML撰写    
目前支持的HTML元素有:<kbd><b><i><em><sup><sub><br/>等使用<kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑
输出结果为：   
使用<kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑

**转义**：Markdown使用了很多符号表示特定的意义，如果需要显示特定的符号则需要使用转义字符，Markdown使用反斜杠转义特殊字符：
**文本加粗**   
\*\*正常显示星号\*\*
_输出结果为：_   
**文本加粗**    
\*\*正常显示星号\*\*
Markdown支持以下这些符号前面加上反斜杠来帮助插入普通的符号：
\   反斜线
`   反引号
*   星号
_   下划线
{}  花括号
[]  方括号
()  小括号
#   井字号
+   加号
-   减号
.   英文句点
!   感叹号
**公式**：   
- 当你需要在编辑器中插入数学公式时，可以使用两个美元符$$包裹 TeX 或 LaTeX 格式的数学公式来实现。提交后，问答和文章页会根据需要加载 Mathjax 对数学公式进行渲染。如：
 $$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
$$tep1}{\style{visibility:hidden}{(x+1)(x+1)}}
$$
输出结果为：   
$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
$$tep1}{\style{visibility:hidden}{(x+1)(x+1)}}
$$
