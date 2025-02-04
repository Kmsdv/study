[TOC]



# 写在前面

## 注意事项

### 切换英文字符

Typora只支持识别英文字符, 所以在撰写笔记的时候要将输入法中的中文字符切换为英文字符

快捷键: `Ctrl` + `.`

![image-20240705191610646](C:\Users\Theresa\AppData\Roaming\Typora\typora-user-images\image-20240705191610646.png)



### 扩展语法

拓展语法, 在Typora上可以使用, 但是有一些编译器并不支持



### 常用的快捷键

|      按键       |        效果        |     按键     |          效果          |
| :-------------: | :----------------: | :----------: | :--------------------: |
|  `Ctrl` + `D`   |     选中当前词     | `Ctrl` + `L` |     选中当前句/行      |
|  `Ctrl` + `E`   |    选中当前区块    | `Ctrl` + `F` |      搜索当前选中      |
|  `Ctrl` + `B`   |    加粗当前选中    | `Ctrl`+ `H`  |      替换当前选中      |
|  `Ctrl` + `I`   |    倾斜当前选中    | `Ctrl` + `U` |      下划当前选中      |
|  `Ctrl` + `K`   | 将当前选中生成链接 | `Ctrl` + `J` | 滚动屏幕将选中滚至底部 |
|  `Ctrl` + `W`   |    关闭当前窗口    | `Ctrl` + `N` |       打开新窗口       |
|  `Ctrl` + `O`   |      打开文件      | `Ctrl` + `P` |     搜索文件并打开     |
| `Ctrl` + `回车` |   表格下方插入行   | `Ctrl` + `,` |      打开偏好设置      |
|  `Ctrl` + `.`   | 切换全角/半角标点  | `Ctrl` + `/` |  切换正常/源代码视图   |

还有许多没有在此列出



# 基础教程

## 1.标题 [数个'#' + 空格  前置]

```
# 一级标题
## 二级标题
### 三级标题
以此类推
```

标题会在大纲和目录分级显示, 可以跳转

注意这个空格是不可缺少的



## 2.强调 [用''**''或"__"包围]

```
**这里是测试文本**
__这里是测试文本__
```

或者选中想要强调的文字按下`Ctrl` + `B`

**这里是测试文本**



## 3.斜体 [用"*"或"_"包围]

```
*这里是测试文本*
_这里是测试文本_
```

或者选中想要强调的文字按下`Ctrl` + `I`

*这里是测试文本*



## 4.斜体并强调 [用"***"或"___"包围]

在此就不过多赘述

***这里是测试文本***



## 5.删除线 [用"~~"包围]

````
~~这里是测试文本~~
````

~~这里是测试文本~~



## 6.高亮 [用"=="包围] (此为扩展语法)

```
==这是测试文本==
```

高亮以及下面会提及到的上标/下标/注释等扩展语法, 需要在`文件`  `偏好设置`  `Markdown`  `Markdown扩展语法` 中选择使用

==这是测试文本==



## 7.代码 [用"`"包围]

```
`这是测试文本`
```

`int main`       `Ctrl`



## 8.代码框 [按三下"`"并敲回车]

```
对就是这个东西
```

想在代码框中显示行号，可以点击`文件`  `偏好设置`  `Markdown`  `代码块`  `显示行号`

代码块中可以显示语言, 起会根据所选择的语言来自动高亮各个语句

```c++
//这段是c++的代码

#include <iostream>
using namespace std;

int main()
{
	cout<<"hello"<<endl;
	return 0;
}
```

```python
///这段是Python代码

print("Hello")
```



## 9.引用 [">" + 空格 前置]

```
> 这是测试文本1
> > 这是测试文本2
```

引用是可以嵌套的! 

> 这是测试文本1
>
> > 这是测试文本2



## 10.无序列表 ["+"或"-" + 空格  前置]

```
+ 这是测试文本1
- 这是测试文本2
* 其实这种也可以, 不过由于在Typora中很难单个输入, 故不常用
```

三种前置符号都可以, 敲回车会自动补全, 可在Typora设置中调整补全的符号, 敲回车之后按下`tab`会缩进一级

+ 这是测试文本1

  + (按下 `tab` 键后)  这是测试文本1

  

## 11.有序列表 [数字 + "." + 空格  前置]

```
我来这里就为了三件事
1. 公平
2. 公平
3. 还是tm的公平!
```

敲回车后会自动补全, 敲回车后按下 `tab` 会缩进一级

我来这里就为了三件事

1. 公平
2. 公平
   1. (按下 `tab` 键后) 还是tm的公平! 



## 12.上标 [用"^"包围] (此为扩展语法)

```
C语言中 int 的上限为 2^31^ -1 = 2147483647
```

C语言中 int 的上限为 2^31^ -1 = 2147483647



## 13.下标 [用 "~"包围] (此为扩展语法)

```
H~2~O是剧毒的
```

H~2~O是剧毒的



## 14.注释 ["[^]" 后置] (此为扩展语法)

```
> 这波我们打野不在我为什么要去你告诉我[^1]

[^1]:传奇中单选手 电棍otto
```

> 这波我们打野不在我为什么要去你告诉我[^1]

[^1]:传奇中单选手 电棍otto



## 15.链接 [常用"[]" + "()"分别包围文本和链接] (文内跳转为扩展语法)

```
[关注瓶子君152喵](https://space.bilibili.com/730732?spm_id_from=333.337.0.0)
[基础教程: 13. 下标](#13.下标 [用 "~"包围] (此为扩展语法))
```

支持网页链接和文内跳转, 按住 `Ctrl` 并 `单击鼠标左键` 即可跳转

[关注瓶子君152喵](https://space.bilibili.com/730732?spm_id_from=333.337.0.0)
[基础教程: 13. 下标](#13.下标 [用 "~"包围] (此为扩展语法))

(注意在文内跳转时标题前面只能有一个 `#` )



## 16.任务列表 ["-[]" + 空格  前置]

```
任务:
- [ ] 虚构叙事
- [ ] 忘却之庭
- [x] 模拟宇宙
```

用 `x` 代替 `[ ]`中的空格来勾选任务, 在Typora中可以直接用鼠标左键单击勾选框

任务:

- [ ] 虚构叙事
- [ ] 忘却之庭
- [x] 模拟宇宙



## 17.表格 [用"|"绘制表格边框]

```
| 角色 | 命途 | 属性 |
|:---|:---:|---:| (引号的位置分别代表 左对齐 居中 右对齐)
|刃|毁灭|风|
|阮·梅|同协|冰|
```

第一行为表头, 第二行决定对齐方式和长度, 第三行及之后为表格数据

| 角色  | 命途 | 属性 |
| :---- | :--: | ---: |
| 刃    | 毁灭 |   风 |
| 阮·梅 | 同协 |   冰 |

在表格中, 你可以按 `Ctrl` + `Enter` 或者直接按 `Tab` 新建新的一行

添加或者删除列则需要在一个表格单元格上点击右键，在上下文菜单中，有添加/删除表格列的菜单项



## 18.图片 [直接拖进来或者复制粘贴   没啥好说的]

<img src="C:\Users\Theresa\Documents\Tencent Files\3038763186\nt_qq\nt_data\Pic\2024-07\Ori\bed3956a9018783c28f139967fe5e294.png" alt="bed3956a9018783c28f139967fe5e294" style="zoom: 25%;" />

值得注意的是,这里拖进来的图片是作为本地文件存储的, 对于共享文档来说会非常不好操作



## 19.分割线 [按三个"*" 或"-" 或"_"并敲回车]

```
***
---
_

```

由于 `*` 和 `_`均会自动补全, 因此个人觉得 `-`最方便

---



## 20.Emoji表情 [":"前置] (英文输入为扩展语法)

```
:sweat_smile:
:clown_face:

//敲回车或者鼠标点击
```

这个功能唯一的要求是英文水平要高 (tm的英语还在追我) , 或者大概记得各个Emoji的英文名

:sweat_smile:

:clown_face:

对于其他的Markdown编辑器, 可以选择直接将Emoji表情复制进来, 这个是硬编码的

---

---

# 进阶教程

## 1.目录 [自动生成]

```
[TOC](在这个文档的开头的目录就是这样实现的)
```

vs code因为我没有用过它的Markdown, 所以我不是很清楚



## 2.内联 HTML 代码 [用"<></>"包围]

```
呃呃,我真不会写 HTML, 等哪天我学成归来了再把这里补全吧
```

Markdown 完全可以当成 **HTML**来写 ~~(虽然我不会就是了)~~

同时, `.md` 文件可以直接导出成一个网页



## 3.内联$\LaTeX$公式 [用"$"符号包围]

```
$\LaTeX$真的很好用

$a^n+b^n=c^n$
```

用 `$` 包围为单条公式, 按下两个 `$` 并敲回车即生成公式块 ~~(因为能力有限这个就不写了)~~

**每个编辑器对公式的支持程度都不一样, 所以$\LaTeX$有的时候会在其他编辑器上无法显示**

$\LaTeX$真的很好用

$a^n+b^n=c^n$



## 4.网络图床 [只是写在这里我根本不知道怎么用]



---

---

