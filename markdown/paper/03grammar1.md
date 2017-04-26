# MarkDown 语法 1

环境准备：
- 在自己的 Github 个人主页创建 MarkDown 仓库，带 README.md；  
- 在某个磁盘下面创建一个文件夹（例如：Github），专门放各种 Github 仓库，不放别的文件夹；  
- git clone 刚创建的 MarkDown 仓库；  
- MarkDown 文件夹用于创建教学演示的 md 文件；  
- 在本地 MarkDown 文件夹中创建 images 文件夹，此文件夹用于放置教学演示需要的图片；  
- 在 HBuilder 中打开 MarkDown 文件夹；  
- 在 MarkDown 文件夹中新建 demo1.md 文件；  
- 在 demo1.md 文件放置本次课程讲的段落、标题、强调和列表这些 MarkDown 语法；
- 内容涉及我的个人信息，包括：各种联系方式，课程信息，希望大家给课程五分评价，等营销信息；  
- 其他内容参考果冻虾仁的文档：https://github.com/guodongxiaren/README

## 段落

如果你了解 HTML。估计你能猜到，刚编写的文档被解释成下面的代码：

```html
<p>Hello, world!</p>
```

段落之间需要用空行隔开，所以，如果你需要创建两个或多个段落，你需要这样编写文档：

```
这是第一个段落。

这是第二个段落。
```

## 标题

标题语法可以很好的帮助我们对信息做分类，她是很重要的语法。

如果你需要添加一个标题，只需要在一行文字的开头输入 `#` 字符。`#` 字符的数量代表标题的级别。例如：

    # 标题 1
    ## 标题 2
    ### 标题 3
    #### 标题 4
    ##### 标题 5
    ###### 标题 6

在 HTML 中，有六种级别的标题。MarkDown 中的标题会根据级别被翻译成 `<h1>`-`<h6>` 相应的 HTML 标记。

一级标题和二级标题还有另一种等价的语法。如在一行文字下面输入三个 `=` 号，则创建了一个一级标题。
在一行文字下面输入三个 `-` 号，则创建了一个二级标题。例如：

    标题 1
    ===

    标题 2
    ---

## 强调

很容易把文字格式化成 _斜体_, **粗体**, _**加粗斜体**_ 以及 ~~删除样式~~。在 MarkDown 中只有几种强调文字的语法，每种语法的可读性都很强。

强调文字只需要把被强调的文字包裹在一个、两个或者三个星号（`*`）或者下划线（`_`）中即可。下面是一些例子：

    使用*星号*或者_下划线_来格式化斜体。

**|>** 使用*星号*或者_下划线_来格式化斜体。

    使用**星号**或者__下划线__来格式化粗体。

**|>** 使用**星号**或者__下划线__来格式化粗体。

    混合使用**星号和 _下划线_**。

**|>** 混合使用**星号和 _下划线_**。

有些时候你需要在文字上划删除线。把需要格式化的文字包裹上两个波浪线（`~`）。像下面这样：

    ~~删除此行。~~

**|>** ~~删除此行。~~

现在你已经知道在 MarkDown 语法中如何轻松的强调重要信息了。

我们建议你对斜体和粗体使用不同的标记，例如：

1. 一个下划线的`_斜体_`和两个星号的`**粗体**`
2. 一个星号的`*斜体*`和两个下划线的`__粗体__`

这种方式可以让你在文档中快速的识别不同的样式。对于_**加粗斜体**_，两种方式你可以自由选择`_**加粗斜体**_`或`*__加粗斜体__*`。

## 列表

列表是一种很重要的结构化信息。用 MarkDown 语法创建列表非常容易。只要在每个项目之前插入一个星号（`*`）或者横线（`-`）就可以创建一个无序列表。在数字后面跟着点号就可以创建一个有序列表（例如：1., 2., 3.）。

### 无序列表

一个无序列表的例子：

    * 项目 1
    * 项目 2
    * 项目 3

格式化后的样子如下：

* 项目 1
* 项目 2
* 项目 3

横线作用相同：

    - 用横线的第一个项目
    - 用横线的第二个项目

结果：

- 用横线的第一个项目
- 用横线的第二个项目

### 有序列表

一个简单的有序列表的例子：

    1. 项目 1
    2. 项目 2
    3. 项目 3

格式化后的样子如下：

1. 项目 1
2. 项目 2
3. 项目 3

正如你所见，这些标记非常直观可读。

### 多级列表

创建多级列表也很简单。只需要像下面这样添加 tab 或空格缩进即可。

    - 项目 1
      - 项目 1.2
      - 项目 1.3
    - 项目 2
      - 项目 2.1
    - 项目 3

使用 `*` 号或有序列表一样能正常工作。

额外强调一下，你可以在有序列表中按任意顺序编排项目。请参考下面的例子：

    0. only zeros
    0. only zeros
    0. only zeros

    10. any order
    5. any order
    2. any order
    7. any order

格式化后的效果如下：

0. only zeros
0. only zeros
0. only zeros

5. any order
10. any order
2. any order
7. any order

Markdown 很聪明，会创建一个正确的顺序。在你维护一个很大的列表时，这个功能非常有用。