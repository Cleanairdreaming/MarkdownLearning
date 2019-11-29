MarkDown语法简介
=============================

下面是Markdwown的语法简介，主要是常用功能，非手册大全，部分内容摘抄自网络，侵权来信删除。  

## 目录
- [MarkDown语法简介](#markdown语法简介)
  - [目录](#目录)
  - [一、标题](#一标题)
    - [1 Setext形式](#1-setext形式)
    - [2 atx形式](#2-atx形式)
  - [二、强调](#二强调)
  - [三、列表](#三列表)
    - [无序列表](#无序列表)
    - [有序列表](#有序列表)
  - [四、链接](#四链接)
  - [五、块引用](#五块引用)
  - [六、行内代码](#六行内代码)
  - [七、语法高亮](#七语法高亮)
  - [八、任务列表](#八任务列表)
  - [九、表格](#九表格)
  - [十 分割线](#十-分割线)


## 一、标题  

### 1 Setext形式  
代码  
```markdown
H1
===
H2
---
=和-的数量无限制，只支持两级标题。
```  

### 2 atx形式  
代码  
```markdown  
# 一级标题
## 二级标题
###### 6级标题
```  


## 二、强调  
```markdown
斜体、黑体及两者结合
*This text will be italic*
_This will also be italic_

**This text will be bold**
__This will also be bold__

_You **can** combine them_
```  
`>>>`  
*This text will be italic*
_This will also be italic_

**This text will be bold**
__This will also be bold__

_You **can** combine them_

## 三、列表  
### 无序列表  
```
* Item 1
* Item 2
  * Item 2a
  * Item 2b
```  
`>>>`  
* Item 1
* Item 2
  * Item 2a
  * Item 2b

### 有序列表  
```
1. Item 1
2. Item 2
3. Item 3
   1. Item 3a
   2. Item 3b
```
`>>>`  
1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b

## 四、链接  
```
Markdown format: 
![Alt Text](url)
![logo](/images/logo.png)

Html format:
<img src="url" width="75" hegiht="75" align=center />
```  
`>>>`  
![logo](/images/logo.png)  
<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" width="75" hegiht="75" align=center />  

## 五、块引用
```
As Kanye West said:
> We're living the future so
> the present is our past.
```  
`>>>`  
As Kanye West said:  
> We're living the future so  
> the present is our past.  

## 六、行内代码
```
I think you should use an `<addr>` element here instead.
```
`>>>`  
I think you should use an `<addr>` element here instead.  

## 七、语法高亮
```python
# ```python
# <python script>
# ```

# python with syntax highlighting
def test(a, b=1, *args):
    sum_ = a + b
    for arg in args:
        sum_ += arg
    return sum_, locals()
sum_, locals_ = test(1, 2, 3, 4)
>>>print(sum)
10
>>>print(locals)
{'arg': 4, 'sum_': 10, 'args': (3, 4), 'b': 2, 'a': 1}
```

```
# python without syntax highlighting
def test(a, b=1, *args):
    sum_ = a + b
    for arg in args:
        sum_ += arg
    return sum_, locals()
sum_, locals_ = test(1, 2, 3, 4)
>>>print(sum)
10
>>>print(locals)
{'arg': 4, 'sum_': 10, 'args': (3, 4), 'b': 2, 'a': 1}
```

## 八、任务列表
```markdown
- [x] @master, :smile:, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
  - [x] HTML
  - [x] CSS
  - [x] JavaScript
- [ ] this is an incomplete item
```  
`>>>`  
- [x] @master, :smile:, [links](#八、任务列表), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
  - [x] HTML
  - [x] CSS
  - [x] JavaScript
- [ ] this is an incomplete item  

Emoji 可参考[Github emoji](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)和[webfx](https://www.webfx.com/tools/emoji-cheat-sheet/)

## 九、表格
* Markdown synopsis  
1）|、-、:之间的多余空格会被忽略，不影响布局。  
2）默认标题栏居中对齐，内容居左对齐。  
3）-:表示内容和标题栏居右对齐，:-表示内容和标题栏居左对齐，:-:表示内容和标题栏居中对齐。  
4）内容和|之间的多余空格会被忽略，每行第一个|和最后一个|可以省略，-的数量至少有一个。  
表格1-4条的语法参考[橡皮24的简书博客](https://www.jianshu.com/p/b0f56b7d7ee8)  

```markdown
First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

| First Header | Second Header  |  
| ------------ | -------------  |  
| Content from cell 1 | Content from cell 2  |  
| Content in the first column | Content in the second column  | 

| First Header | Second Header  |  
| :-: | :-: |  
| Content from cell 1 | Content from cell 2  |  
| Content in the first column | Content in the second column  | 

Important! Empty line need before the table.
```
`>>>`  

| First Header | Second Header  |  
| ------------ | -------------  |  
| Content from cell 1 | Content from cell 2  |  
| Content in the first column | Content in the second column  |  

| First Header | Second Header  |  
| :-: | :-: |  
| Content from cell 1 | Content from cell 2  |  
| Content in the first column | Content in the second column  | 

* Html supported
```html
<!-- use html Synopis instead -->
<table border="1">  
  <tr>  
    <th>Month</th>  
    <th>Savings</th>  
  </tr>  
  <tr>  
    <td>January</td>  
    <td>$100</td>  
  </tr>  
</table> 
```
`>>>`  
<table border="1">  
  <tr>  
    <th>Month</th>  
    <th>Savings</th>  
  </tr>  
  <tr>  
    <td>January</td>  
    <td>$100</td>  
  </tr>  
</table>  

## 十 分割线
```
---
or
***
```
---

***