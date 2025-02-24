# Markdown-
前言：虽然我已经写过不少md笔记，但是偶尔还是会学到或者忘记某些知识，所以这里会记录一些相关知识。
---
### 1.在 Markdown (md) 格式中，可以通过输入三个或更多的短横线（-）、星号（*）或下划线（_），并且每个符号之间可以有空格，来创建分界线（水平线）。
eg：
```Markdown
---
***
___
```

---

### 2.Markdown 之所以可以使用 HTML 标签，是因为 Markdown 语言本质上是一种轻量级的标记语言，旨在通过简单的语法格式化文本，同时允许嵌入原生的 HTML 代码。这种设计使得 Markdown 既易于书写，又具有灵活性，可以处理更复杂的格式需求。

---

### 3.在Markdown中，可以使用双星号 ** 或者双下划线 __ 来表示粗体文本。

示例：

使用双星号：**这是粗体文本**

使用双下划线：__这是粗体文本__

渲染效果：

这是粗体文本

---

### 4.在 GitHub Markdown 中要实现分行显示但不留空行，可以使用以下两种方式：

方法 1：行尾双空格（推荐）  
学生表 (Student)  
StudentID (学生ID，主键)  
StudentName (学生姓名)  

方法 2：HTML 换行标签  
学生表 (Student)<br>
StudentID (学生ID，主键)<br>
StudentName (学生姓名)

两种方式效果相同，最终渲染效果为：  
学生表 (Student)  
StudentID (学生ID，主键)  
StudentName (学生姓名)  

原理说明：

1、在 Markdown 中，普通换行会被合并成单个空格

2、行尾添加两个空格会触发硬换行（对应 HTML 的 &lt;br&gt; 标签）

3、这是 GitHub Flavored Markdown (GFM) 的标准特性

4、建议优先使用双空格方案，这是 Markdown 的原生语法

---

### 5.在 GitHub 上的 Markdown 文档中，HTML 标签（包括 <br>）会被直接渲染。你想让 <br> 显示为文字而不是换行，可以通过转义字符 &lt;br&gt; 来实现。

具体方法：  
你可以这样写：

2、行尾添加两个空格会触发硬换行（对应 HTML 的 &lt;br&gt; 标签）

解释：  
&lt; 和 &gt; 是 < 和 > 的 HTML 转义字符，表示将这些字符作为文本显示，而不是 HTML 标签。  
这样，<br> 会作为普通文本显示在 GitHub 文档中，而不会引发换行。  

结果：  
在 GitHub 上渲染出来时，会看到类似如下的内容：

2、行尾添加两个空格会触发硬换行（对应 HTML 的 <br> 标签）  
这会让 <br> 以文本形式显示，而不会被解释为换行标签。
